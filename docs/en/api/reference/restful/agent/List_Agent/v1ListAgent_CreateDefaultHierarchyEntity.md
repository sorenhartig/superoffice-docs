---
title: POST Agents/List/CreateDefaultHierarchyEntity
uid: v1ListAgent_CreateDefaultHierarchyEntity
---

# POST Agents/List/CreateDefaultHierarchyEntity

```http
POST /api/v1/Agents/List/CreateDefaultHierarchyEntity
```

Set default values into a new HierarchyEntity.


NetServer calculates default values on the entity, which is required when creating/storing a new instance







## Request Headers

| Parameter Name | Description |
|----------------|-------------|
| Authorization  | Supports 'Basic', 'SoTicket' and 'Bearer' schemes, depending on installation type. |
| X-XSRF-TOKEN   | If not using Authorization header, you must provide XSRF value from cookie or hidden input field |
| Accept         | Content-type(s) you would like the response in: `application/json`, `text/json`, `application/xml`, `text/xml`, `application/json-patch+json`, `application/merge-patch+json` |
| Accept-Language | Convert string references and multi-language values into a specified language (iso2) code. |
| SO-Language | Convert string references and multi-language values into a specified language (iso2) code. Overrides Accept-Language value. |
| SO-Culture | Number, date formatting in a specified culture (iso2 language) code. Partially overrides SO-Language/Accept-Language value. Ignored if no Language set. |
| SO-TimeZone | Specify the timezone code that you would like date/time responses converted to. |
| SO-AppToken | The application token that identifies the partner app. Used when calling Online WebAPI from a server. |


## Response:

OK

| Response | Description |
|----------------|-------------|
| 200 | OK |

### Response body: HierarchyEntity

| Property Name | Type |  Description |
|----------------|------|--------------|
| HierarchyId | int32 | The primary key (auto-incremented) |
| Domain | string | Domain seperating the different hierarchy |
| Name | string | Name of this hierarchy folder. |
| Fullname | string | The full name of this category, i.e. Foo/bar/test. |
| ParentId | int32 | Parent table |
| Children | array | Sub-items, if any. |
| Registered | date-time | Registered when  in UTC. |
| RegisteredAssociateId | int32 | Registered by whom |
| Updated | date-time | Last updated when  in UTC. |
| UpdatedAssociateId | int32 | Last updated by whom |
| TableRight | TableRight |  |
| FieldProperties | object |  |

## Sample request

```http!
POST /api/v1/Agents/List/CreateDefaultHierarchyEntity
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: *
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "HierarchyId": 915,
  "Domain": "Dashboards",
  "Name": "Weissnat, Kuhic and Jones",
  "Fullname": "id",
  "ParentId": 965,
  "Children": [
    {
      "HierarchyId": 235,
      "Domain": "Dashboards",
      "Name": "White-Lang",
      "Fullname": "repellat",
      "ParentId": 731,
      "Children": [
        {},
        {}
      ],
      "Registered": "2011-05-07T17:37:18.276242+02:00",
      "RegisteredAssociateId": 449,
      "Updated": "2018-03-24T17:37:18.276242+01:00",
      "UpdatedAssociateId": 125,
      "TableRight": null,
      "FieldProperties": {
        "fieldName": {
          "FieldRight": null,
          "FieldType": "System.Int32",
          "FieldLength": 159
        }
      }
    }
  ],
  "Registered": "1999-06-05T17:37:18.276242+02:00",
  "RegisteredAssociateId": 87,
  "Updated": "2020-09-14T17:37:18.276242+02:00",
  "UpdatedAssociateId": 398,
  "TableRight": null,
  "FieldProperties": {
    "fieldName": {
      "FieldRight": null,
      "FieldType": "System.String",
      "FieldLength": 631
    }
  }
}
```