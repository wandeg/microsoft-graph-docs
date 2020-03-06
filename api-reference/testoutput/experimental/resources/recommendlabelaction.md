---
title: "recommendLabelAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# recommendLabelAction resource type


Namespace: microsoft.graph




Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[informationProtectionAction](../resources/informationprotectionaction.md) collection||
|actionSource|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`, `default`.|
|label|[labelDetails](../resources/labeldetails.md)||
|responsibleSensitiveTypeIds|Guid collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recommendLabelAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendLabelAction",
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

