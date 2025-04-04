---
title: POST Agents/EMail/GetEmailAppointmentRecurrence
uid: v1EMailAgent_GetEmailAppointmentRecurrence
---

# POST Agents/EMail/GetEmailAppointmentRecurrence

```http
POST /api/v1/Agents/EMail/GetEmailAppointmentRecurrence
```

Get recurrence data contained in the email iCal attachment


## Online Restricted: ## The EMail agent is not available in Online by default. Access must be requested specifically when app is registered.






## Query String Parameters

| Parameter Name | Type |  Description |
|----------------|------|--------------|
| $select | string |  Optional comma separated list of properties to include in the result. Other fields are then nulled out to reduce payload size: "Name,department,category". Default = show all fields. |

```http
POST /api/v1/Agents/EMail/GetEmailAppointmentRecurrence?$select=name,department,category/id
```


## Request Headers

| Parameter Name | Description |
|----------------|-------------|
| Authorization  | Supports 'Basic', 'SoTicket' and 'Bearer' schemes, depending on installation type. |
| X-XSRF-TOKEN   | If not using Authorization header, you must provide XSRF value from cookie or hidden input field |
| Content-Type | Content-type of the request body: `application/json`, `text/json`, `application/xml`, `text/xml`, `application/x-www-form-urlencoded`, `application/json-patch+json`, `application/merge-patch+json` |
| Accept         | Content-type(s) you would like the response in: `application/json`, `text/json`, `application/xml`, `text/xml`, `application/json-patch+json`, `application/merge-patch+json` |
| Accept-Language | Convert string references and multi-language values into a specified language (iso2) code. |
| SO-Language | Convert string references and multi-language values into a specified language (iso2) code. Overrides Accept-Language value. |
| SO-Culture | Number, date formatting in a specified culture (iso2 language) code. Partially overrides SO-Language/Accept-Language value. Ignored if no Language set. |
| SO-TimeZone | Specify the timezone code that you would like date/time responses converted to. |
| SO-AppToken | The application token that identifies the partner app. Used when calling Online WebAPI from a server. |

## Request Body: request 

MailItemId 

| Property Name | Type |  Description |
|----------------|------|--------------|
| MailItemId | Integer |  |

## Response:

OK

| Response | Description |
|----------------|-------------|
| 200 | OK |

### Response body: TableRight

| Property Name | Type |  Description |
|----------------|------|--------------|
| RecurrenceId | int32 |  |
| StartDate | date-time |  |
| EndDate | date-time |  |
| RecurrenceCounter | int32 |  |
| RecurrenceEndType | string |  |
| Pattern | string |  |
| DayPattern | TableRight |  |
| WeekPattern | TableRight |  |
| MonthPattern | TableRight |  |
| YearPattern | TableRight |  |
| Dates | array |  |
| IsRecurrence | bool |  |

## Sample request

```http!
POST /api/v1/Agents/EMail/GetEmailAppointmentRecurrence
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: fr,de,ru,zh
Content-Type: application/json; charset=utf-8

{
  "MailItemId": 164
}
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "RecurrenceId": 720,
  "StartDate": "2013-07-30T17:37:17.8972444+02:00",
  "EndDate": "2006-02-20T17:37:17.8972444+01:00",
  "RecurrenceCounter": 159,
  "RecurrenceEndType": "Counter",
  "Pattern": "Custom",
  "DayPattern": null,
  "WeekPattern": null,
  "MonthPattern": null,
  "YearPattern": null,
  "Dates": [
    {
      "Date": "2006-02-21T17:37:17.8972444+01:00",
      "IsConflict": true,
      "Description": "Upgradable radical product",
      "DescriptionStyleHint": "Managed fresh-thinking local area network",
      "Tooltip": "aut"
    },
    {
      "Date": "2006-02-21T17:37:17.8972444+01:00",
      "IsConflict": true,
      "Description": "Upgradable radical product",
      "DescriptionStyleHint": "Managed fresh-thinking local area network",
      "Tooltip": "aut"
    }
  ],
  "IsRecurrence": false
}
```