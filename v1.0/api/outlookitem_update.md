# Update outlookitem

Update the properties of outlookitem object.
### Prerequisites
One of the following **scopes** is required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http

```
### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|categories|String||
|changeKey|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||

### Response
If successful, this method returns a `200 OK` response code and updated [outlookItem](../resources/outlookitem.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_outlookitem"
}-->
```http

Content-type: application/json
Content-length: 165

{
  "createdDateTime": "datetime-value",
  "lastModifiedDateTime": "datetime-value",
  "changeKey": "changeKey-value",
  "categories": [
    "categories-value"
  ]
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookitem"
} -->
```http
Content-type: application/json
Content-length: 185

{
  "createdDateTime": "datetime-value",
  "lastModifiedDateTime": "datetime-value",
  "changeKey": "changeKey-value",
  "categories": [
    "categories-value"
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->