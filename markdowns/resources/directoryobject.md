# DirectoryObject resource type

Represents an Azure Active Directory object. The **DirectoryObject** type is the base type for most of the other directory entity types.

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryobject"
}-->

```json
{
  "Id": "String-value (identifier)"
}

```
### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Id|String| Read-only.|

### Relationships
None


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get DirectoryObject](../api/directoryobject_get.md) | [DirectoryObject](directoryobject.md) |Read properties and relationships of directoryObject object.|
|[Delete](../api/directoryobject_delete.md) | None |Delete DirectoryObject object. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "DirectoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->