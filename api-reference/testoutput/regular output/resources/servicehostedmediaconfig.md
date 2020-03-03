---
title: "serviceHostedMediaConfig resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# serviceHostedMediaConfig resource type




Inherits from [mediaConfig](../resources/mediaConfig.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|preFetchMedia|[mediaInfo](../resources/mediaInfo.md) collection||

## Relationships
None

## JSON Representation
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

