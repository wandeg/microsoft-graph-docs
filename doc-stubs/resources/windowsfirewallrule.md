---
title: "windowsFirewallRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsFirewallRule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|stateManagementSetting|**TODO: Add Description**. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|edgeTraversal|stateManagementSetting|**TODO: Add Description**. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|filePath|String|**TODO: Add Description**|
|interfaceTypes|windowsFirewallRuleInterfaceTypes|**TODO: Add Description**. Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|localAddressRanges|String collection|**TODO: Add Description**|
|localPortRanges|String collection|**TODO: Add Description**|
|localUserAuthorizations|String|**TODO: Add Description**|
|packageFamilyName|String|**TODO: Add Description**|
|profileTypes|windowsFirewallRuleNetworkProfileTypes|**TODO: Add Description**. Possible values are: `notConfigured`, `domain`, `private`, `public`.|
|protocol|Int32|**TODO: Add Description**|
|remoteAddressRanges|String collection|**TODO: Add Description**|
|remotePortRanges|String collection|**TODO: Add Description**|
|serviceName|String|**TODO: Add Description**|
|trafficDirection|windowsFirewallRuleTrafficDirectionType|**TODO: Add Description**. Possible values are: `notConfigured`, `out`, `in`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "protocol": "Integer",
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

