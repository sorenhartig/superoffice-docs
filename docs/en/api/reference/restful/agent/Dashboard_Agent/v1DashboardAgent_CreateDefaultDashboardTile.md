---
title: POST Agents/Dashboard/CreateDefaultDashboardTile
uid: v1DashboardAgent_CreateDefaultDashboardTile
---

# POST Agents/Dashboard/CreateDefaultDashboardTile

```http
POST /api/v1/Agents/Dashboard/CreateDefaultDashboardTile
```

Set default values into a new DashboardTile.


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

### Response body: DashboardTile

| Property Name | Type |  Description |
|----------------|------|--------------|
| DashboardTileId | int32 | The tile id |
| Caption | string | The tile caption |
| Description | string | The tile description |
| ChartName | string | The original chart name |
| ChartId | string | The original chart Id |
| IsDefault | bool | True if this is one of the default tiles |
| AssociateId | int32 | Id of the associate who owns this tile |
| GroupId | int32 | Id of the associates primary group at storage time |
| SelectionId | int32 | The selection that defines the data filter/restrictions |
| Config | string | The tile config |
| Type | string | The tile type, what kind of tile this is |
| EntityType | string | The tile entity type |
| Options | array | The tile options |
| VisibleFor | array | The set of users or groups the record is visible for |
| TableRight | TableRight |  |
| FieldProperties | object |  |

## Sample request

```http!
POST /api/v1/Agents/Dashboard/CreateDefaultDashboardTile
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: en
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "DashboardTileId": 293,
  "Caption": "accusamus",
  "Description": "User-centric dynamic info-mediaries",
  "ChartName": "Crona, Wunsch and Kris",
  "ChartId": "voluptas",
  "IsDefault": true,
  "AssociateId": 248,
  "GroupId": 350,
  "SelectionId": 119,
  "Config": "eius",
  "Type": "Bignum",
  "EntityType": "Activity",
  "Options": [
    {
      "Name": "Goldner-Paucek",
      "Description": "Cloned next generation implementation",
      "Type": "Boolean",
      "ListName": "Dibbert Inc and Sons",
      "ListItems": [
        {},
        {}
      ],
      "Value": "soluta",
      "DefaultDataOption": true,
      "TableRight": null,
      "FieldProperties": {
        "fieldName": {
          "FieldRight": null,
          "FieldType": "System.String",
          "FieldLength": 81
        }
      }
    }
  ],
  "VisibleFor": [
    {
      "VisibleId": 395,
      "Visibility": "All",
      "DisplayValue": "sunt",
      "TableRight": null,
      "FieldProperties": {
        "fieldName": {
          "FieldRight": null,
          "FieldType": "System.String",
          "FieldLength": 720
        }
      }
    },
    {
      "VisibleId": 395,
      "Visibility": "All",
      "DisplayValue": "sunt",
      "TableRight": null,
      "FieldProperties": {
        "fieldName": {
          "FieldRight": null,
          "FieldType": "System.String",
          "FieldLength": 720
        }
      }
    }
  ],
  "TableRight": null,
  "FieldProperties": {
    "fieldName": {
      "FieldRight": null,
      "FieldType": "System.Int32",
      "FieldLength": 152
    }
  }
}
```