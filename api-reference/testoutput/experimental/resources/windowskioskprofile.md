---
title: "windowsKioskProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsKioskProfile resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appConfiguration|[windowsKioskAppConfiguration](../resources/windowsKioskAppConfiguration.md)|The App configuration that will be used for this kiosk configuration.|
|profileId|String|Key of the entity.|
|profileName|String|This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.|
|userAccountsConfiguration|[windowsKioskUser](../resources/windowsKioskUser.md) collection|The user accounts that will be locked to this kiosk configuration. This collection can contain a maximum of 100 elements.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskAppConfiguration"
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```

