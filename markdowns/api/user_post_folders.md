# Create Folder

Use this API to create a new Folder.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Folders
POST /Users/<Id>/Folders

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [Folder](../resources/folder.md) object.


### Response
If successful, this method returns `201, Created` response code and [Folder](../resources/folder.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_folder_from_user"
}-->
```http
POST https://outlook.office.com/v1.0/me
```
In the request body, supply a JSON representation of [Folder](../resources/folder.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.folder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Folder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->