---
title: "informationProtectionPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# informationProtectionPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get informationProtectionPolicy](../api/informationprotectionpolicy-get.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Read properties and relationships of the [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[Update informationProtectionPolicy](../api/informationprotectionpolicy-update.md)|[informationProtectionPolicy](../resources/informationprotectionpolicy.md)|Update the properties of a [informationProtectionPolicy](../resources/informationprotectionpolicy.md) object.|
|[List labels](../api/informationprotectionpolicy-list-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md) collection|Get the informationProtectionLabels from the labels navigation property.|
|[Add labels](../api/informationprotectionpolicy-post-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Add labels by posting to the labels collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|labels|[informationProtectionLabel](../resources/informationprotectionlabel.md) collection||

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

