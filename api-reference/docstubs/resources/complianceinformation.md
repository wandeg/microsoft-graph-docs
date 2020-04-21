---
title: "complianceInformation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# complianceInformation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificationControls|[certificationControl](../resources/certificationcontrol.md) collection|**TODO: Add Description**|
|certificationName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceInformation",
  "certificationControls": [
    {
      "@odata.type": "microsoft.graph.certificationControl",
      "name": "String",
      "url": "String"
    }
  ],
  "certificationName": "String"
}
```

