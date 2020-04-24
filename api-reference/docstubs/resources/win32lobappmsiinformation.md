---
title: "win32LobAppMsiInformation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppMsiInformation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|packageType|win32LobAppMsiPackageType|The MSI package type. Possible values are: `perMachine`, `perUser`, `dualPurpose`.|
|productCode|String|The MSI product code.|
|productName|String|The MSI product name.|
|productVersion|String|The MSI product version.|
|publisher|String|The MSI publisher.|
|requiresReboot|Boolean|Whether the MSI app requires the machine to reboot to complete installation.|
|upgradeCode|String|The MSI upgrade code.|

## Relationships
None

## JSON representation
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

