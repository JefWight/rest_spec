# Update folder

Update the properties of folder object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/RootFolder
PATCH /me/Folders/<Id>
PATCH /Users/<Id>/RootFolder
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolderCount|Int32||
|DisplayName|String||
|ParentFolderId|String||
|TotalItemCount|Int32||
|UnreadItemCount|Int32||

### Response
If successful, this method returns a `200 OK` response code and updated [Folder](../resources/folder.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_folder"
}-->
```http
PUT https://outlook.office.com/v1.0/me/RootFolder
Content-type: application/json
Content-length: 179

{
  "DisplayName": "DisplayName-value",
  "ParentFolderId": "ParentFolderId-value",
  "ChildFolderCount": 99,
  "UnreadItemCount": 99,
  "TotalItemCount": 99,
  "Id": "Id-value"
}
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.folder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "DisplayName": "DisplayName-value",
  "ParentFolderId": "ParentFolderId-value",
  "ChildFolderCount": 99,
  "UnreadItemCount": 99,
  "TotalItemCount": 99,
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update folder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->