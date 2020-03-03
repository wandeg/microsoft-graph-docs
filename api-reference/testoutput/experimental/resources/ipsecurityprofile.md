---
title: "ipSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# ipSecurityProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get ipSecurityProfile](../api/ipsecurityprofile-get.md)|[ipSecurityProfile](../resources/ipSecurityProfile.md)|Read properties and relationships of the [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|
|[Delete ipSecurityProfile](../api/ipsecurityprofile-delete.md)|None|Deletes a [ipSecurityProfile](../resources/ipsecurityprofile.md).|
|[Update ipSecurityProfile](../api/ipsecurityprofile-update.md)|[ipSecurityProfile](../resources/ipSecurityProfile.md)|Update the properties of a [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|
|[List ipSecurityProfiles](../api/security-list-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipSecurityProfile.md) collection|Get the ipSecurityProfiles from the ipSecurityProfiles navigation property.|
|[Add ipSecurityProfiles](../api/security-post-ipsecurityprofiles.md)|[ipSecurityProfile](../resources/ipSecurityProfile.md)|Add ipSecurityProfiles by posting to the ipSecurityProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection||
|address|String||
|azureSubscriptionId|String||
|azureTenantId|String||
|countHits|Int32||
|countHosts|Int32||
|firstSeenDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipCategories|[ipCategory](../resources/ipCategory.md) collection||
|ipReferenceData|[ipReferenceData](../resources/ipReferenceData.md) collection||
|lastSeenDateTime|DateTimeOffset||
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
  "@odata.type": "microsoft.graph.ipSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "id": "String (identifier)",
  "activityGroupNames": [
    "String"
  ],
  "address": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "countHits": 1024,
  "countHosts": 1024,
  "firstSeenDateTime": "String (timestamp)",
  "ipCategories": [
    {
      "@odata.type": "microsoft.graph.ipCategory"
    }
  ],
  "ipReferenceData": [
    {
      "@odata.type": "microsoft.graph.ipReferenceData"
    }
  ],
  "lastSeenDateTime": "String (timestamp)",
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

