---
title: "hostSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hostSecurityProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|fqdn|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isAzureAdJoined|Boolean|**TODO: Add Description**|
|isAzureAdRegistered|Boolean|**TODO: Add Description**|
|isHybridAzureDomainJoined|Boolean|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|logonUsers|[logonUser](../resources/logonuser.md) collection|**TODO: Add Description**|
|netBiosName|String|**TODO: Add Description**|
|networkInterfaces|[networkInterface](../resources/networkinterface.md) collection|**TODO: Add Description**|
|os|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|parentHost|String|**TODO: Add Description**|
|relatedHostIds|String collection|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hostSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "id": "String (identifier)",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "firstSeenDateTime": "String (timestamp)",
  "fqdn": "String",
  "isAzureAdJoined": "Boolean",
  "isAzureAdRegistered": "Boolean",
  "isHybridAzureDomainJoined": "Boolean",
  "lastSeenDateTime": "String (timestamp)",
  "logonUsers": [
    {
      "@odata.type": "microsoft.graph.logonUser"
    }
  ],
  "netBiosName": "String",
  "networkInterfaces": [
    {
      "@odata.type": "microsoft.graph.networkInterface"
    }
  ],
  "os": "String",
  "osVersion": "String",
  "parentHost": "String",
  "relatedHostIds": [
    "String"
  ],
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

