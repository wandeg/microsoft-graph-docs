---
title: "hostSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# hostSecurityProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get hostSecurityProfile](../api/hostsecurityprofile-get.md)|[hostSecurityProfile](../resources/hostSecurityProfile.md)|Read properties and relationships of the [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[Delete hostSecurityProfile](../api/hostsecurityprofile-delete.md)|None|Deletes a [hostSecurityProfile](../resources/hostsecurityprofile.md).|
|[Update hostSecurityProfile](../api/hostsecurityprofile-update.md)|[hostSecurityProfile](../resources/hostSecurityProfile.md)|Update the properties of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.|
|[List hostSecurityProfiles](../api/security-list-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostSecurityProfile.md) collection|Get the hostSecurityProfiles from the hostSecurityProfiles navigation property.|
|[Add hostSecurityProfiles](../api/security-post-hostsecurityprofiles.md)|[hostSecurityProfile](../resources/hostSecurityProfile.md)|Add hostSecurityProfiles by posting to the hostSecurityProfiles collection.|

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
|logonUsers|[logonUser](../resources/logonUser.md) collection||
|netBiosName|String||
|networkInterfaces|[networkInterface](../resources/networkInterface.md) collection||
|os|String||
|osVersion|String||
|parentHost|String||
|relatedHostIds|String collection||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||

## Relationships
None

## JSON Representation
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

