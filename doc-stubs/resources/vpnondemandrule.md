---
title: "vpnOnDemandRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vpnOnDemandRule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|vpnOnDemandRuleConnectionAction|**TODO: Add Description**. Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|dnsSearchDomains|String collection|**TODO: Add Description**|
|domainAction|vpnOnDemandRuleConnectionDomainAction|**TODO: Add Description**. Possible values are: `connectIfNeeded`, `neverConnect`.|
|domains|String collection|**TODO: Add Description**|
|probeRequiredUrl|String|**TODO: Add Description**|
|probeUrl|String|**TODO: Add Description**|
|ssids|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

