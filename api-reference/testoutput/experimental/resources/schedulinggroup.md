---
title: "schedulingGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# schedulingGroup resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get schedulingGroup](../api/schedulinggroup-get.md)|[schedulingGroup](../resources/schedulingGroup.md)|Read properties and relationships of the [schedulingGroup](../resources/schedulinggroup.md) object.|
|[Delete schedulingGroup](../api/schedulinggroup-delete.md)|None|Deletes a [schedulingGroup](../resources/schedulinggroup.md).|
|[Update schedulingGroup](../api/schedulinggroup-update.md)|[schedulingGroup](../resources/schedulingGroup.md)|Update the properties of a [schedulingGroup](../resources/schedulinggroup.md) object.|
|[List schedulingGroups](../api/schedule-list-schedulinggroups.md)|[schedulingGroup](../resources/schedulingGroup.md) collection|Get the schedulingGroups from the schedulingGroups navigation property.|
|[Add schedulingGroups](../api/schedule-post-schedulinggroups.md)|[schedulingGroup](../resources/schedulingGroup.md)|Add schedulingGroups by posting to the schedulingGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isActive|Boolean||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|userIds|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.schedulingGroup",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "String",
  "isActive": true,
  "userIds": [
    "String"
  ]
}
```

