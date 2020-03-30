---
title: "sharedAppleDeviceUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharedAppleDeviceUser resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataQuota|Int64||
|dataToSync|Boolean||
|dataUsed|Int64||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```

