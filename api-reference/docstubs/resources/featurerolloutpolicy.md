---
title: "featureRolloutPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# featureRolloutPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get featureRolloutPolicy](../api/featurerolloutpolicy-get.md)|[featureRolloutPolicy](../resources/featurerolloutpolicy.md)|Read the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.|
|[Update featureRolloutPolicy](../api/featurerolloutpolicy-update.md)|[featureRolloutPolicy](../resources/featurerolloutpolicy.md)|Update the properties of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.|
|[List appliesTo](../api/featurerolloutpolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/featurerolloutpolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create a new appliesTo object.|
|[Delete appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)|None|Delete an [directoryObject](../resources/directoryobject.md) object.|
|[Update appliesTo](../api/featurerolloutpolicy-update-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of an appliesTo object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read the properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|feature|stagedFeatureName|**TODO: Add Description**. Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAppliedToOrganization|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.featureRolloutPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "feature": "String",
  "isEnabled": true,
  "isAppliedToOrganization": true
}
```

