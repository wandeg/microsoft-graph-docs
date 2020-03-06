---
title: "windowsKioskAzureADGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskAzureADGroup resource type


Namespace: microsoft.graph




Inherits from [windowsKioskUser](../resources/windowskioskuser.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name of the AzureAD group that will be locked to this kiosk configuration|
|groupId|String|The ID of the AzureAD group that will be locked to this kiosk configuration|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```

