---
title: "win32LobAppProductCodeDetection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobAppProductCodeDetection resource type


Namespace: microsoft.graph




Inherits from [win32LobAppDetection](../resources/win32lobappdetection.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|productCode|String|The product code of Win32 Line of Business (LoB) app.|
|productVersion|String|The product version of Win32 Line of Business (LoB) app.|
|productVersionOperator|Enumeration|The operator to detect product version. Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```

