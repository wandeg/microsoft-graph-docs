---
title: "androidDeviceOwnerGlobalProxyDirect resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidDeviceOwnerGlobalProxyDirect resource type


Namespace: microsoft.graph




Inherits from [androidDeviceOwnerGlobalProxy](../resources/androiddeviceownerglobalproxy.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludedHosts|String collection|The excluded hosts|
|host|String|The host name|
|port|Int32|The port|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```

