---
title: "informationProtectionPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# informationProtectionPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get informationProtectionPolicy](../api/informationprotectionpolicy-get.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Read the properties and relationships of an [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[Update informationProtectionPolicy](../api/informationprotectionpolicy-update.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Update the properties of an [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[List labels](../api/informationprotectionpolicy-list-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md) collection|Get the informationProtectionLabels from the labels navigation property.|
|[Create labels](../api/informationprotectionpolicy-post-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Create a new labels object.|
|[Delete labels](../api/informationprotectionpolicy-delete-labels.md)|None|Delete a [informationProtectionLabel](../resources/informationprotectionlabel.md) object.|
|[Update labels](../api/informationprotectionpolicy-update-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Update the properties of a labels object.|
|[Get informationProtectionLabel](../api/informationprotectionlabel-get.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Read the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.|
|[List policy](../api/informationprotection-list-policy.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md) collection|Get the informationProtectionPolicies from the policy navigation property.|
|[Create policy](../api/informationprotection-post-policy.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Create a new policy object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|labels|[informationProtectionLabel](../resources/informationprotectionlabel.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.informationProtectionPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.informationProtectionPolicy",
  "id": "String (identifier)"
}
```

