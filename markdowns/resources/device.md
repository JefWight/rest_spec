# Device resource type



#### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|accountEnabled|Boolean||
|alternativeSecurityIds|[AlternativeSecurityId](alternativesecurityid.md) collection||
|approximateLastLogonTimestamp|DateTimeOffset||
|deletionTimestamp|DateTimeOffset||
|deviceId|Guid||
|deviceMetadata|String||
|deviceOSType|String||
|deviceOSVersion|String||
|deviceObjectVersion|Int32||
|devicePhysicalIds|String collection||
|deviceTrustType|String||
|dirSyncEnabled|Boolean||
|displayName|String||
|lastDirSyncTime|DateTimeOffset||
|objectId|String| Read-only.|
|objectType|String||

#### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Extensions|[Extension](extension.md) collection| Read-only.|
|registeredOwners|[DirectoryObject](directoryobject.md) collection| Read-only.|
|registeredUsers|[DirectoryObject](directoryobject.md) collection| Read-only.|

#### Tasks

| Task		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Device](../api/device_get.md) | Device |Read properties and relationships of device object.|
|[Create Extension]((../api/device_post_extensions.md)) |Extension| Create a new Extension by posting to the Extensions collection.|
|[Create DirectoryObject]((../api/device_post_registeredowners.md)) |DirectoryObject| Create a new DirectoryObject by posting to the registeredOwners collection.|
|[Create DirectoryObject]((../api/device_post_registeredusers.md)) |DirectoryObject| Create a new DirectoryObject by posting to the registeredUsers collection.|
|[Update](../api/device_update.md) | Device	|Update Device object. |
|[Delete](../api/device_delete.md) | Device	|Delete Device object. |
|[Checkmembergroups](../api/device_checkmembergroups.md)|String||
|[Get getMemberGroups](../api/device_getmembergroups.md)|String||
|[Get getMemberObjects](../api/device_getmemberobjects.md)|String||