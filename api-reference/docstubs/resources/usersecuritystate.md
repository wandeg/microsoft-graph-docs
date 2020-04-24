---
title: "userSecurityState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userSecurityState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aadUserId|String|**TODO: Add Description**|
|accountName|String|**TODO: Add Description**|
|domainName|String|**TODO: Add Description**|
|emailRole|emailRole|**TODO: Add Description**. Possible values are: `unknown`, `sender`, `recipient`, `unknownFutureValue`.|
|isVpn|Boolean|**TODO: Add Description**|
|logonDateTime|DateTimeOffset|**TODO: Add Description**|
|logonId|String|**TODO: Add Description**|
|logonIp|String|**TODO: Add Description**|
|logonLocation|String|**TODO: Add Description**|
|logonType|logonType|**TODO: Add Description**. Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`, `unknownFutureValue`.|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|userAccountType|userAccountSecurityType|**TODO: Add Description**. Possible values are: `unknown`, `standard`, `power`, `administrator`, `unknownFutureValue`.|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSecurityState",
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "String",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "String",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "String",
  "userPrincipalName": "String"
}
```

