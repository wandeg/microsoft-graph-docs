---
title: "identityContainer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# identityContainer resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get identityContainer](../api/identitycontainer-get.md)|[identityContainer](../resources/identitycontainer.md)|Read the properties and relationships of an [identityContainer](../resources/identitycontainer.md) object.|
|[Update identityContainer](../api/identitycontainer-update.md)|[identityContainer](../resources/identitycontainer.md)|Update the properties of an [identityContainer](../resources/identitycontainer.md) object.|
|[List conditionalAccess](../api/identitycontainer-list-conditionalaccess.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md) collection|Get the conditionalAccessRoots from the conditionalAccess navigation property.|
|[Create conditionalAccess](../api/identitycontainer-post-conditionalaccess.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Create a new conditionalAccess object.|
|[Delete conditionalAccess](../api/identitycontainer-delete-conditionalaccess.md)|None|Delete a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[Update conditionalAccess](../api/identitycontainer-update-conditionalaccess.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Update the properties of a conditionalAccess object.|
|[Get conditionalAccessRoot](../api/conditionalaccessroot-get.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Read the properties and relationships of a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[List userFlows](../api/identitycontainer-list-userflows.md)|[identityUserFlow](../resources/identityuserflow.md) collection|Get the identityUserFlows from the userFlows navigation property.|
|[Create userFlows](../api/identitycontainer-post-userflows.md)|[identityUserFlow](../resources/identityuserflow.md)|Create a new userFlows object.|
|[Delete userFlows](../api/identitycontainer-delete-userflows.md)|None|Delete a [identityUserFlow](../resources/identityuserflow.md) object.|
|[Update userFlows](../api/identitycontainer-update-userflows.md)|[identityUserFlow](../resources/identityuserflow.md)|Update the properties of a userFlows object.|
|[Get identityUserFlow](../api/identityuserflow-get.md)|[identityUserFlow](../resources/identityuserflow.md)|Read the properties and relationships of an [identityUserFlow](../resources/identityuserflow.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|conditionalAccess|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|**TODO: Add Description**|
|userFlows|[identityUserFlow](../resources/identityuserflow.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

