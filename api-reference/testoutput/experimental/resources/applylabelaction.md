---
title: "applyLabelAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# applyLabelAction resource type




Inherits from [informationProtectionAction](../resources/informationProtectionAction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[informationProtectionAction](../resources/informationProtectionAction.md) collection||
|actionSource|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`, `default`.|
|label|[labelDetails](../resources/labelDetails.md)||
|responsibleSensitiveTypeIds|Guid collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.applyLabelAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applyLabelAction",
  "label": {
    "@odata.type": "microsoft.graph.labelDetails",
    "id": "String",
    "name": "String",
    "description": "String",
    "color": "String",
    "sensitivity": 1024,
    "tooltip": "String",
    "isActive": true
  },
  "responsibleSensitiveTypeIds": [
    "Guid"
  ],
  "actions": [
    {
      "@odata.type": "microsoft.graph.addContentFooterAction",
      "uiElementName": "String",
      "text": "String",
      "fontName": "String",
      "fontSize": 1024,
      "fontColor": "String",
      "alignment": "String",
      "margin": 1024
    }
  ],
  "actionSource": "String"
}
```

