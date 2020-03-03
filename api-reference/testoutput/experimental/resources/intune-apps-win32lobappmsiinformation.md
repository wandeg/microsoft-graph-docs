---
title: "win32LobAppMsiInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# win32LobAppMsiInformation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|packageType|Enumeration|The MSI package type. Possible values are: `perMachine`, `perUser`, `dualPurpose`.|
|productCode|String|The MSI product code.|
|productName|String|The MSI product name.|
|productVersion|String|The MSI product version.|
|publisher|String|The MSI publisher.|
|requiresReboot|Boolean|Whether the MSI app requires the machine to reboot to complete installation.|
|upgradeCode|String|The MSI upgrade code.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```

