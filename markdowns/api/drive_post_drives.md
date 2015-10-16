# Create drive

Use this API to create a new drive.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /drives

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [drive](../resources/drive.md) object.


### Response
If successful, this method returns `201, Created` response code and [drive](../resources/drive.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_drive_from_drives"
}-->
```http
POST /drives
Content-type: application/json
```
In the request body, supply a JSON representation of [drive](../resources/drive.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "drive"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 458
{
  "id": "id-value",
  "driveType": "driveType-value",
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
  },
  "quota": {
    "deleted": 99,
    "remaining": 99,
    "state": "state-value",
    "total": 99,
    "used": 99
  }
}
```

<!-- uuid: 6c74e1e0-828a-4191-9ba4-702cea76999c
2015-10-16 10:07:51 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create drive",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->