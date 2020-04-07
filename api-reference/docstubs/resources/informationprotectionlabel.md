---
title: "informationProtectionLabel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# informationProtectionLabel resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get informationProtectionLabel](../api/informationprotectionlabel-get.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Read properties and relationships of the [informationProtectionLabel](../resources/informationprotectionlabel.md) object.|
|[Update informationProtectionLabel](../api/informationprotectionlabel-update.md)|[informationProtectionLabel](../resources/informationprotectionlabel.md)|Update the properties of a [informationProtectionLabel](../resources/informationprotectionlabel.md) object.|
|[extractLabel](../api/informationprotectionlabel-extractlabel.md)|[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)||
|[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection||
|[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection||
|[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)|[informationProtectionAction](../resources/informationprotectionaction.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isActive|Boolean||
|name|String||
|sensitivity|Int32||
|tooltip|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "sensitivity": 1024,
  "tooltip": "String",
  "isActive": true
}
```

