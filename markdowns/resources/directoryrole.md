# DirectoryRole resource type



#### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|deletionTimestamp|DateTimeOffset||
|description|String||
|displayName|String||
|isSystem|Boolean||
|objectId|String| Read-only.|
|objectType|String||
|roleDisabled|Boolean||
|roleTemplateId|String||

#### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Extensions|[Extension](extension.md) collection| Read-only.|
|memberOf|[DirectoryObject](directoryobject.md) collection| Read-only.|
|members|[DirectoryObject](directoryobject.md) collection| Read-only.|
|ownedObjects|[DirectoryObject](directoryobject.md) collection| Read-only.|
|owners|[DirectoryObject](directoryobject.md) collection| Read-only.|

#### Tasks

| Task		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get DirectoryRole](../api/directoryrole_get.md) | DirectoryRole |Read properties and relationships of directoryRole object.|
|[Create Extension]((../api/directoryrole_post_extensions.md)) |Extension| Create a new Extension by posting to the Extensions collection.|
|[Create DirectoryObject]((../api/directoryrole_post_memberof.md)) |DirectoryObject| Create a new DirectoryObject by posting to the memberOf collection.|
|[Create DirectoryObject]((../api/directoryrole_post_members.md)) |DirectoryObject| Create a new DirectoryObject by posting to the members collection.|
|[Create DirectoryObject]((../api/directoryrole_post_ownedobjects.md)) |DirectoryObject| Create a new DirectoryObject by posting to the ownedObjects collection.|
|[Create DirectoryObject]((../api/directoryrole_post_owners.md)) |DirectoryObject| Create a new DirectoryObject by posting to the owners collection.|
|[Update](../api/directoryrole_update.md) | DirectoryRole	|Update DirectoryRole object. |
|[Delete](../api/directoryrole_delete.md) | DirectoryRole	|Delete DirectoryRole object. |
|[Checkmembergroups](../api/directoryrole_checkmembergroups.md)|String||
|[Get getMemberGroups](../api/directoryrole_getmembergroups.md)|String||
|[Get getMemberObjects](../api/directoryrole_getmemberobjects.md)|String||