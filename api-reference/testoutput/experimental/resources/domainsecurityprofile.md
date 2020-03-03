---
title: "domainSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# domainSecurityProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get domainSecurityProfile](../api/domainsecurityprofile-get.md)|[domainSecurityProfile](../resources/domainSecurityProfile.md)|Read properties and relationships of the [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[Delete domainSecurityProfile](../api/domainsecurityprofile-delete.md)|None|Deletes a [domainSecurityProfile](../resources/domainsecurityprofile.md).|
|[Update domainSecurityProfile](../api/domainsecurityprofile-update.md)|[domainSecurityProfile](../resources/domainSecurityProfile.md)|Update the properties of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[List domainSecurityProfiles](../api/security-list-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainSecurityProfile.md) collection|Get the domainSecurityProfiles from the domainSecurityProfiles navigation property.|
|[Add domainSecurityProfiles](../api/security-post-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainSecurityProfile.md)|Add domainSecurityProfiles by posting to the domainSecurityProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|countHits|Int32||
|countInOrg|Int32||
|domainCategories|[reputationCategory](../resources/reputationCategory.md) collection||
|domainRegisteredDateTime|DateTimeOffset||
|firstSeenDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSeenDateTime|DateTimeOffset||
|name|String||
|registrant|[domainRegistrant](../resources/domainRegistrant.md)||
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

