---
title: "vpnOnDemandRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vpnOnDemandRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration| Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|dnsSearchDomains|String collection||
|domainAction|Enumeration| Possible values are: `connectIfNeeded`, `neverConnect`.|
|domains|String collection||
|probeRequiredUrl|String||
|probeUrl|String||
|ssids|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```

