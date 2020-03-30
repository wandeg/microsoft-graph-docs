---
title: "identityContainer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identityContainer resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityContainer](../api/identitycontainer-get.md)|[identityContainer](../resources/identitycontainer.md)|Read properties and relationships of the [identityContainer](../resources/identitycontainer.md) object.|
|[Update identityContainer](../api/identitycontainer-update.md)|[identityContainer](../resources/identitycontainer.md)|Update the properties of a [identityContainer](../resources/identitycontainer.md) object.|
|[Get conditionalAccessRoot](../api/conditionalaccessroot-get.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Read properties and relationships of the [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[List userFlows](../api/identitycontainer-list-userflows.md)|[identityUserFlow](../resources/identityuserflow.md) collection|Get the identityUserFlows from the userFlows navigation property.|
|[Add userFlows](../api/identitycontainer-post-userflows.md)|[identityUserFlow](../resources/identityuserflow.md)|Add userFlows by posting to the userFlows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|conditionalAccess|[conditionalAccessRoot](../resources/conditionalaccessroot.md)||
|userFlows|[identityUserFlow](../resources/identityuserflow.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityContainer",
  "id": "String (identifier)"
}
```

