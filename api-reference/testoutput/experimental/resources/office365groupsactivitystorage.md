---
title: "office365GroupsActivityStorage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# office365GroupsActivityStorage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365GroupsActivityStorages](../api/office365groupsactivitystorage-list.md)|[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) collection|List properties and relationships of the [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) objects.|
|[Get office365GroupsActivityStorage](../api/office365groupsactivitystorage-get.md)|[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)|Read properties and relationships of the [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object.|
|[Create office365GroupsActivityStorage](../api/office365groupsactivitystorage-create.md)|[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)|Create a new [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object.|
|[Delete office365GroupsActivityStorage](../api/office365groupsactivitystorage-delete.md)|None|Deletes a [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md).|
|[Update office365GroupsActivityStorage](../api/office365groupsactivitystorage-update.md)|[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)|Update the properties of a [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mailboxStorageUsedInBytes|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|siteStorageUsedInBytes|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365GroupsActivityStorage",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "mailboxStorageUsedInBytes": 1024,
  "siteStorageUsedInBytes": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

