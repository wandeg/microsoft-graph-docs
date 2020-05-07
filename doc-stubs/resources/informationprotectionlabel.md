---
title: "informationProtectionLabel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# informationProtectionLabel resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[extractLabel](../api/informationprotectionlabel-extractlabel.md)|[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)|**TODO: Add Description**|
|[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection|**TODO: Add Description**|
|[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection|**TODO: Add Description**|
|[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection|**TODO: Add Description**|
|[List labels](../api/informationprotectionpolicy-list-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md) collection|Get the informationProtectionLabels from the labels navigation property.|
|[Create labels](../api/informationprotectionpolicy-post-labels.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Create a new labels object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isActive|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|sensitivity|Int32|**TODO: Add Description**|
|tooltip|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.informationProtectionLabel",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "color": "String",
  "sensitivity": "Integer",
  "tooltip": "String",
  "isActive": "Boolean"
}
```

