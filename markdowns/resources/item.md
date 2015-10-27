# Item resource type

The Item resource type represents metadata for an item in OneDrive. All top-level filesystem objects in OneDrive are Item resources. If an item is a [Folder](../facets/folder_facet.md) or [File](../facets/file_facet.md) facet, the Item resource will contain a value for either the **folder** or **file** property, respectively.  

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.item"
}-->

```json
{
  "Categories": [
    "String-value"
  ],
  "ChangeKey": "String-value",
  "DateTimeCreated": "String (timestamp)",
  "DateTimeLastModified": "String (timestamp)",
  "Id": "String-value (identifier)"
}

```
### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Categories|String collection||
|ChangeKey|String||
|DateTimeCreated|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|DateTimeLastModified|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Id|String|The unique identifier of the item within the Drive. Read-only. Read-only.|

### Relationships
None


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Item](../api/item_get.md) | [Item](item.md) |Read properties and relationships of item object.|
|[Update](../api/item_update.md) | [Item](item.md)	|Update Item object. |
|[Delete](../api/item_delete.md) | None |Delete Item object. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->