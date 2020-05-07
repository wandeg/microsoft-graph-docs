---
title: "iosNotificationSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosNotificationSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alertType|iosNotificationAlertType|**TODO: Add Description**. Possible values are: `deviceDefault`, `banner`, `modal`, `none`.|
|appName|String|**TODO: Add Description**|
|badgesEnabled|Boolean|**TODO: Add Description**|
|bundleID|String|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|showInNotificationCenter|Boolean|**TODO: Add Description**|
|showOnLockScreen|Boolean|**TODO: Add Description**|
|soundsEnabled|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "enabled": "Boolean",
  "showInNotificationCenter": "Boolean",
  "showOnLockScreen": "Boolean",
  "alertType": "String",
  "badgesEnabled": "Boolean",
  "soundsEnabled": "Boolean"
}
```

