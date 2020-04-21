---
title: "mediaStream resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# mediaStream resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|direction|mediaDirection|**TODO: Add Description**. Possible values are: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.|
|label|String|**TODO: Add Description**|
|mediaType|modality|**TODO: Add Description**. Possible values are: `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|serverMuted|Boolean|**TODO: Add Description**|
|sourceId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaStream"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaStream",
  "mediaType": "String",
  "label": "String",
  "sourceId": "String",
  "direction": "String",
  "serverMuted": true
}
```

