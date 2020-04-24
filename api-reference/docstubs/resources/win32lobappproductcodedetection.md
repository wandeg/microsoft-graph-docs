---
title: "win32LobAppProductCodeDetection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppProductCodeDetection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [win32LobAppDetection](../resources/win32lobappdetection.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|productCode|String|The product code of Win32 Line of Business (LoB) app.|
|productVersion|String|The product version of Win32 Line of Business (LoB) app.|
|productVersionOperator|win32LobAppDetectionOperator|The operator to detect product version. Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|

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

