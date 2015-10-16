# Update the properties of share object.

Update the properties of share object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /shares/<id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|name|String||
|owner|identitySet||

### Response
If successful, this method returns a `200 OK` response code and updated [share](../resources/share.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_share"
}-->
```http
PUT /shares/<id>
Content-type: application/json
Content-length: 330
{
  "id": "id-value",
  "name": "name-value",
  "owner": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  }
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "share"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 330
{
  "id": "id-value",
  "name": "name-value",
  "owner": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  }
}
```

<!-- uuid: 1e481e20-e0d9-4b19-9b3e-ad132b7cc39f
2015-10-16 10:08:05 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of share object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->