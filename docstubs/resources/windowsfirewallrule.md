---
title: "windowsFirewallRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsFirewallRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Possible values are: `notConfigured`, `blocked`, `allowed`.|
|description|String||
|displayName|String||
|edgeTraversal|Enumeration| Possible values are: `notConfigured`, `blocked`, `allowed`.|
|filePath|String||
|interfaceTypes|Enumeration| Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|localAddressRanges|String collection||
|localPortRanges|String collection||
|localUserAuthorizations|String||
|packageFamilyName|String||
|profileTypes|Enumeration| Possible values are: `notConfigured`, `domain`, `private`, `public`.|
|protocol|Int32||
|remoteAddressRanges|String collection||
|remotePortRanges|String collection||
|serviceName|String||
|trafficDirection|Enumeration| Possible values are: `notConfigured`, `out`, `in`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```

