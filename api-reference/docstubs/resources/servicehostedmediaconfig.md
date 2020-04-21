---
title: "serviceHostedMediaConfig resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# serviceHostedMediaConfig resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [mediaConfig](../resources/mediaconfig.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|preFetchMedia|[mediaInfo](../resources/mediainfo.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  "preFetchMedia": [
    {
      "@odata.type": "microsoft.graph.mediaInfo",
      "uri": "String",
      "resourceId": "String"
    }
  ]
}
```

