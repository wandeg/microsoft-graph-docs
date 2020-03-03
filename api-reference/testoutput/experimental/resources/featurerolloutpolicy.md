---
title: "featureRolloutPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# featureRolloutPolicy resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get featureRolloutPolicy](../api/featurerolloutpolicy-get.md)|[featureRolloutPolicy](../resources/featureRolloutPolicy.md)|Read properties and relationships of the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.|
|[Delete featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)|None|Deletes a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).|
|[Update featureRolloutPolicy](../api/featurerolloutpolicy-update.md)|[featureRolloutPolicy](../resources/featureRolloutPolicy.md)|Update the properties of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.|
|[List appliesTo](../api/featurerolloutpolicy-list-appliesto.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/featurerolloutpolicy-post-appliesto.md)|[directoryObject](../resources/directoryObject.md)|Add appliesTo by posting to the appliesTo collection.|
|[List featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md)|[featureRolloutPolicy](../resources/featureRolloutPolicy.md) collection|Get the featureRolloutPolicies from the featureRolloutPolicies navigation property.|
|[Add featureRolloutPolicies](../api/directory-post-featurerolloutpolicies.md)|[featureRolloutPolicy](../resources/featureRolloutPolicy.md)|Add featureRolloutPolicies by posting to the featureRolloutPolicies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|feature|Enumeration|. Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isAppliedToOrganization|Boolean||
|isEnabled|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryObject.md) collection||

## JSON Representation
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

