---
title: "recommendLabelAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# recommendLabelAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [informationProtectionAction](../resources/informationprotectionaction.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[informationProtectionAction](../resources/informationprotectionaction.md) collection|**TODO: Add Description**|
|actionSource|actionSource|**TODO: Add Description**. Possible values are: `manual`, `automatic`, `recommended`, `default`.|
|label|[labelDetails](../resources/labeldetails.md)|**TODO: Add Description**|
|responsibleSensitiveTypeIds|Guid collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recommendLabelAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendLabelAction",
  "label": {
    "@odata.type": "microsoft.graph.labelDetails"
  },
  "responsibleSensitiveTypeIds": [
    "Guid"
  ],
  "actions": [
    {
      "@odata.type": "microsoft.graph.addContentFooterAction"
    }
  ],
  "actionSource": "String"
}
```

