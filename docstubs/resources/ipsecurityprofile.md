---
title: "ipSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# ipSecurityProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get ipSecurityProfile](../api/ipsecurityprofile-get.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Read properties and relationships of the [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|
|[Update ipSecurityProfile](../api/ipsecurityprofile-update.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Update the properties of a [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|

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
|ipCategories|[ipCategory](../resources/ipcategory.md) collection||
|ipReferenceData|[ipReferenceData](../resources/ipreferencedata.md) collection||
|lastSeenDateTime|DateTimeOffset||
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

