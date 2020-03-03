---
title: "scopedRoleMembership resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# scopedRoleMembership resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List scopedRoleMemberships](../api/scopedrolemembership-list.md)|[scopedRoleMembership](../resources/scopedrolemembership.md) collection|List properties and relationships of the [scopedRoleMembership](../resources/scopedrolemembership.md) objects.|
|[Get scopedRoleMembership](../api/scopedrolemembership-get.md)|[scopedRoleMembership](../resources/scopedrolemembership.md)|Read properties and relationships of the [scopedRoleMembership](../resources/scopedrolemembership.md) object.|
|[Create scopedRoleMembership](../api/scopedrolemembership-post-scopedrolememberships.md)|[scopedRoleMembership](../resources/scopedrolemembership.md)|Create a new [scopedRoleMembership](../resources/scopedrolemembership.md) object.|
|[Delete scopedRoleMembership](../api/scopedrolemembership-delete.md)|None|Deletes a [scopedRoleMembership](../resources/scopedrolemembership.md).|
|[Update scopedRoleMembership](../api/scopedrolemembership-update.md)|[scopedRoleMembership](../resources/scopedrolemembership.md)|Update the properties of a [scopedRoleMembership](../resources/scopedrolemembership.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|administrativeUnitId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|roleId|String||
|roleMemberInfo|[identity](../resources/identity.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopedRoleMembership",
  "id": "String (identifier)",
  "roleId": "String",
  "administrativeUnitId": "String",
  "roleMemberInfo": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

