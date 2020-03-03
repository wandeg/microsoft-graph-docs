---
title: "iosStoreAppAssignmentSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosStoreAppAssignmentSettings resource type


Namespace: microsoft.graph




Inherits from [mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|uninstallOnDeviceRemoval|Boolean|Whether or not to uninstall the app when device is removed from Intune.|
|vpnConfigurationId|String|The VPN Configuration Id to apply for this app.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```

