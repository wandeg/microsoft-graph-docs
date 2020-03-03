---
title: "clientUserAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# clientUserAgent resource type




Inherits from [userAgent](../resources/userAgent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationVersion|String| Inherited from [userAgent](../resources/callRecords-userAgent.md)|
|headerValue|String| Inherited from [userAgent](../resources/callRecords-userAgent.md)|
|platform|Enumeration|. Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `iPPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|Enumeration|. Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
  "headerValue": "String",
  "applicationVersion": "String",
  "platform": "String",
  "productFamily": "String"
}
```

