# List PrivilegedOperationEvent

Retrieve a list of privilegedoperationevent objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /PrivilegedOperationEvents
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. See relationships table of [PrivilegedOperationEvent](../resources/privilegedoperationevent.md) for supported names. |
|$filter|string|Filter string that lets you filter the response based on a set of criteria.|
|$orderby|string|Comma-separated list of properties that are used to sort the order of items in the response collection.|
|$select|string|Comma-separated list of properties to include in the response.|
|$skip|int|The number of items to skip in a result set.|
|$skipToken|string|Paging token that is used to get the next set of results.|
|$top|int|The number of items to return in a result set.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [PrivilegedOperationEvent](../resources/privilegedoperationevent.md) objects in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "privilegedoperationevents"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 538
{
  "values": [
    {
      "Id": "Id-value",
      "UserId": "UserId-value",
      "UserName": "UserName-value",
      "UserMail": "UserMail-value",
      "RoleId": "RoleId-value",
      "RoleName": "RoleName-value",
      "ExpirationTime": "datetime-value",
      "CreationTime": "datetime-value",
      "RequestorId": "RequestorId-value",
      "RequestorName": "RequestorName-value",
      "TenantId": "TenantId-value",
      "RequestType": "RequestType-value",
      "AdditionalInformation": "AdditionalInformation-value"
    }
  ]
}
```
If successful, this method returns a `200 OK` response code and collection of [PrivilegedOperationEvent](../resources/privilegedoperationevent.md) objects in the response body.

<!-- uuid: 2b86f026-af6b-400d-8cb5-9058cc3c0b0e
2015-10-16 10:08:02 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List PrivilegedOperationEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->