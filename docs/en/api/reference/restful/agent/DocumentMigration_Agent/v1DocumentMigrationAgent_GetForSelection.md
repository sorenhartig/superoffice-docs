---
title: POST Agents/DocumentMigration/GetForSelection
uid: v1DocumentMigrationAgent_GetForSelection
---

# POST Agents/DocumentMigration/GetForSelection

```http
POST /api/v1/Agents/DocumentMigration/GetForSelection
```

Gets a migration summary for documents in the provided selection


## Online Restricted: ## The DocumentMigration agent is not available in Online by default. Access must be requested specifically when app is registered. Intended for SuperOffice-internal apps.






## Query String Parameters

| Parameter Name | Type |  Description |
|----------------|------|--------------|
| $select | string |  Optional comma separated list of properties to include in the result. Other fields are then nulled out to reduce payload size: "Name,department,category". Default = show all fields. |

```http
POST /api/v1/Agents/DocumentMigration/GetForSelection?$select=name,department,category/id
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

DocumentPluginId, SelectionId, IncludeEmails 

| Property Name | Type |  Description |
|----------------|------|--------------|
| DocumentPluginId | Integer |  |
| SelectionId | Integer |  |
| IncludeEmails | Boolean |  |

## Response:

OK

| Response | Description |
|----------------|-------------|
| 200 | OK |

### Response body: DocumentMigrationItemList

| Property Name | Type |  Description |
|----------------|------|--------------|
| NumDocumentsOmitted | int32 | Total amount of documents within the selection criteria, which has been omitted from the migration. |
| NumDocumentsAlreadyMigrated | int32 | Documents already migrated to the requested documentplugin. |
| Documents | array | List of documents to be migrated. |
| Associates | array | List of associates whose documents will be migrated. |

## Sample request

```http!
POST /api/v1/Agents/DocumentMigration/GetForSelection
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: fr,de,ru,zh
Content-Type: application/json; charset=utf-8

{
  "DocumentPluginId": 514,
  "SelectionId": 595,
  "IncludeEmails": false
}
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "NumDocumentsOmitted": 430,
  "NumDocumentsAlreadyMigrated": 921,
  "Documents": [
    {
      "DocumentId": 800,
      "ContactId": 915,
      "PersonId": 85,
      "SaleId": 69,
      "ProjectId": 176,
      "DocTmplId": 610,
      "AssociateId": 636,
      "UserGroupId": 363,
      "VisibleForId": 61
    }
  ],
  "Associates": [
    {
      "AssociateId": 90,
      "EmailAddress": "doris.schmidt@turcotte.info"
    },
    {
      "AssociateId": 90,
      "EmailAddress": "doris.schmidt@turcotte.info"
    }
  ]
}
```