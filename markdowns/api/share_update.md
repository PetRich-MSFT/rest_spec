# Update share

Update the properties of share object.
### HTTP request
```http
PATCH /shares/<id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP headers used by the API could be displayed.|

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
```http
PUT /shares/<id>
Content-type: application/json
Content-length: 64
{
  "id": "id-value",
  "name": "name-value",
  "owner": {
  }
}
```
##### Response
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64
{
  "id": "id-value",
  "name": "name-value",
  "owner": {
  }
}
```

<!-- uuid: 66cd87ba-a1ff-44f2-ab1b-f82d5bc72a52
2015-10-09 18:16:07 UTC -->