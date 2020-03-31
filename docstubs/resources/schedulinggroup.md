---
title: "schedulingGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# schedulingGroup resource type


Namespace: microsoft.graph




Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get schedulingGroup](../api/schedulinggroup-get.md)|[schedulingGroup](../resources/schedulinggroup.md)|Read properties and relationships of the [schedulingGroup](../resources/schedulinggroup.md) object.|
|[Update schedulingGroup](../api/schedulinggroup-update.md)|[schedulingGroup](../resources/schedulinggroup.md)|Update the properties of a [schedulingGroup](../resources/schedulinggroup.md) object.|
|[List schedulingGroups](../api/schedule-list-schedulinggroups.md)|[schedulingGroup](../resources/schedulinggroup.md) collection|Get the schedulingGroups from the schedulingGroups navigation property.|
|[Add schedulingGroups](../api/schedule-post-schedulinggroups.md)|[schedulingGroup](../resources/schedulinggroup.md)|Add schedulingGroups by posting to the schedulingGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isActive|Boolean||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|userIds|String collection||

## Relationships
None

## JSON representation
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

