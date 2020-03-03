---
title: "officeClientCheckinStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# officeClientCheckinStatus resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliedPolicies|String collection||
|checkinDateTime|DateTimeOffset||
|deviceName|String||
|devicePlatform|String||
|devicePlatformVersion|String||
|errorMessage|String||
|userId|String||
|userPrincipalName|String||
|wasSuccessful|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```

