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
|action|Enumeration|Action. Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|dnsSearchDomains|String collection|DNS Search Domains.|
|domainAction|Enumeration|Domain Action (Only applicable when Action is evaluate connection). Possible values are: `connectIfNeeded`, `neverConnect`.|
|domains|String collection|Domains (Only applicable when Action is evaluate connection).|
|probeRequiredUrl|String|Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).|
|probeUrl|String|A URL to probe. If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.|
|ssids|String collection|Network Service Set Identifiers (SSIDs).|

## Relationships
None

## JSON Representation
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

