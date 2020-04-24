---
title: "applyLabelAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applyLabelAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[informationProtectionAction](../resources/informationprotectionaction.md) collection|**TODO: Add Description**|
|actionSource|actionSource|**TODO: Add Description**. Possible values are: `manual`, `automatic`, `recommended`, `default`.|
|label|[labelDetails](../resources/labeldetails.md)|**TODO: Add Description**|
|responsibleSensitiveTypeIds|Guid collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

