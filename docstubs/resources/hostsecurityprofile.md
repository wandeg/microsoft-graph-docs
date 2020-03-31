---
title: "hostSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# hostSecurityProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get hostSecurityProfile](../api/hostsecurityprofile-get.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Read properties and relationships of the [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[Update hostSecurityProfile](../api/hostsecurityprofile-update.md)|[hostSecurityProfile](../resources/hostsecurityprofile.md)|Update the properties of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureSubscriptionId|String||
|azureTenantId|String||
|firstSeenDateTime|DateTimeOffset||
|fqdn|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isAzureAdJoined|Boolean||
|isAzureAdRegistered|Boolean||
|isHybridAzureDomainJoined|Boolean||
|lastSeenDateTime|DateTimeOffset||
|logonUsers|[logonUser](../resources/logonuser.md) collection||
|netBiosName|String||
|networkInterfaces|[networkInterface](../resources/networkinterface.md) collection||
|os|String||
|osVersion|String||
|parentHost|String||
|relatedHostIds|String collection||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
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

