---
title: "windowsKioskAzureADUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsKioskAzureADUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsKioskUser](../resources/windowskioskuser.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userId|String|The ID of the AzureAD user that will be locked to this kiosk configuration|
|userPrincipalName|String|The user accounts that will be locked to this kiosk configuration|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```

