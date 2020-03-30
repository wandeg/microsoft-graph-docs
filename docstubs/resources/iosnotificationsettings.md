---
title: "iosNotificationSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosNotificationSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|alertType|Enumeration| Possible values are: `deviceDefault`, `banner`, `modal`, `none`.|
|appName|String||
|badgesEnabled|Boolean||
|bundleID|String||
|enabled|Boolean||
|publisher|String||
|showInNotificationCenter|Boolean||
|showOnLockScreen|Boolean||
|soundsEnabled|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```

