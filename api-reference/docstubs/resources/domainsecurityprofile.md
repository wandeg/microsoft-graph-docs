---
title: "domainSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# domainSecurityProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get domainSecurityProfile](../api/domainsecurityprofile-get.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Read the properties and relationships of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[Update domainSecurityProfile](../api/domainsecurityprofile-update.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Update the properties of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|countHits|Int32|**TODO: Add Description**|
|countInOrg|Int32|**TODO: Add Description**|
|domainCategories|[reputationCategory](../resources/reputationcategory.md) collection|**TODO: Add Description**|
|domainRegisteredDateTime|DateTimeOffset|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|registrant|[domainRegistrant](../resources/domainregistrant.md)|**TODO: Add Description**|
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
  "@odata.type": "microsoft.graph.domainSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainSecurityProfile",
  "id": "String (identifier)",
  "activityGroupNames": [
    "String"
  ],
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "countHits": 1024,
  "countInOrg": 1024,
  "domainCategories": [
    {
      "@odata.type": "microsoft.graph.reputationCategory"
    }
  ],
  "domainRegisteredDateTime": "String (timestamp)",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "name": "String",
  "registrant": {
    "@odata.type": "microsoft.graph.domainRegistrant"
  },
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

