# Folder resource type

A folder in a user's mailbox, such as Inbox, Drafts, and Sent Items. Folders can contain messages and other folders.

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "ChildFolders",
    "Messages"
  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "ChildFolderCount": 1024,
  "ChildFolders": [
    {
      "@odata.type": "microsoft.graph.folder"
    }
  ],
  "DisplayName": "String-value",
  "Id": "String-value (identifier)",
  "Messages": [
    {
      "@odata.type": "microsoft.graph.message"
    }
  ],
  "ParentFolderId": "String-value",
  "TotalItemCount": 1024,
  "UnreadItemCount": 1024
}

```
### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolderCount|Int32||
|DisplayName|String||
|Id|String| Read-only.|
|ParentFolderId|String||
|TotalItemCount|Int32||
|UnreadItemCount|Int32||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolders|[Folder](folder.md) collection| Read-only. Nullable.|
|Messages|[Message](message.md) collection| Read-only. Nullable.|

### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Folder](../api/folder_get.md) | [Folder](folder.md) |Read properties and relationships of folder object.|
|[Create Folder](../api/folder_post_childfolders.md) |[Folder](folder.md)| Create a new Folder by posting to the ChildFolders collection.|
|[List ChildFolders](../api/folder_list_childfolders.md) |[Folder](folder.md) collection| Get a Folder object collection.|
|[Create Message](../api/folder_post_messages.md) |[Message](message.md)| Create a new Message by posting to the Messages collection.|
|[List Messages](../api/folder_list_messages.md) |[Message](message.md) collection| Get a Message object collection.|
|[Update](../api/folder_update.md) | [Folder](folder.md)	|Update Folder object. |
|[Delete](../api/folder_delete.md) | None |Delete Folder object. |
|[Copy](../api/folder_copy.md)|[Folder](folder.md)||
|[Move](../api/folder_move.md)|[Folder](folder.md)||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->