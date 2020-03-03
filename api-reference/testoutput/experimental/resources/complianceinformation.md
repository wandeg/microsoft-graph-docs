---
title: "complianceInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# complianceInformation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificationControls|[certificationControl](../resources/certificationControl.md) collection||
|certificationName|String||

## Relationships
None

## JSON Representation
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

