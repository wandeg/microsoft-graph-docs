---
title: "ipSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ipSecurityProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get ipSecurityProfile](../api/ipsecurityprofile-get.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Read the properties and relationships of an [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|
|[Update ipSecurityProfile](../api/ipsecurityprofile-update.md)|[ipSecurityProfile](../resources/ipsecurityprofile.md)|Update the properties of an [ipSecurityProfile](../resources/ipsecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection|**TODO: Add Description**|
|address|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|countHits|Int32|**TODO: Add Description**|
|countHosts|Int32|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ipCategories|[ipCategory](../resources/ipcategory.md) collection|**TODO: Add Description**|
|ipReferenceData|[ipReferenceData](../resources/ipreferencedata.md) collection|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

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

