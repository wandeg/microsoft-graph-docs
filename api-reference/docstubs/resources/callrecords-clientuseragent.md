---
title: "clientUserAgent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# clientUserAgent resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [userAgent](../resources/useragent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationVersion|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md)|
|headerValue|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md)|
|platform|clientPlatform|**TODO: Add Description**. Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.|
|productFamily|productFamily|**TODO: Add Description**. Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
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

