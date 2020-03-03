---
title: "windowsKioskAzureADUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskAzureADUser resource type


Namespace: microsoft.graph




Inherits from [windowsKioskUser](../resources/windowskioskuser.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userId|String|The ID of the AzureAD user that will be locked to this kiosk configuration|
|userPrincipalName|String|The user accounts that will be locked to this kiosk configuration|

## Relationships
None

## JSON Representation
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

