---
title: DEL List/TicketCategory/Items/{id}
uid: v1TicketCategoryList_DeleteTicketCategoryEntity
---

# DEL List/TicketCategory/Items/{id}

```http
DELETE /api/v1/List/TicketCategory/Items/{id}
```

Marks the existing TicketCategoryEntity as deleted.


Calls the List agent service SaveTicketCategoryEntity.





| Path Part | Type | Description |
|-----------|------|-------------|
| id | int32 | The id of TicketCategoryEntity to be marked as deleted. **Required** |



## Request Headers

| Parameter Name | Description |
|----------------|-------------|
| Authorization  | Supports 'Basic', 'SoTicket' and 'Bearer' schemes, depending on installation type. |
| X-XSRF-TOKEN   | If not using Authorization header, you must provide XSRF value from cookie or hidden input field |
| Accept         | Content-type(s) you would like the response in:  |
| SO-AppToken | The application token that identifies the partner app. Used when calling Online WebAPI from a server. |


## Response:

No Content

| Response | Description |
|----------------|-------------|
| 204 | No Content |

### Response body: RecurrenceInfo


## Sample request

```http!
DELETE /api/v1/List/TicketCategory/Items/{id}
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: en
```

## Sample response

```http_
HTTP/1.1 204 No Content
Content-Type: application/json; charset=utf-8

null
```