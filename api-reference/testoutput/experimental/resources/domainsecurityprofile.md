---
title: "domainSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainSecurityProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainSecurityProfiles](../api/domainsecurityprofile-list.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection|List properties and relationships of the [domainSecurityProfile](../resources/domainsecurityprofile.md) objects.|
|[Get domainSecurityProfile](../api/domainsecurityprofile-get.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Read properties and relationships of the [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[Create domainSecurityProfile](../api/domainsecurityprofile-create.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Create a new [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[Delete domainSecurityProfile](../api/domainsecurityprofile-delete.md)|None|Deletes a [domainSecurityProfile](../resources/domainsecurityprofile.md).|
|[Update domainSecurityProfile](../api/domainsecurityprofile-update.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Update the properties of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.|
|[List domainSecurityProfiles](../api/security-list-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md) collection|Get the domainSecurityProfiles from the domainSecurityProfiles navigation property.|
|[Add domainSecurityProfiles](../api/security-post-domainsecurityprofiles.md)|[domainSecurityProfile](../resources/domainsecurityprofile.md)|Add domainSecurityProfiles by posting to the domainSecurityProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupNames|String collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|countHits|Int32||
|countInOrg|Int32||
|domainCategories|[reputationCategory](../resources/reputationcategory.md) collection||
|domainRegisteredDateTime|DateTimeOffset||
|firstSeenDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSeenDateTime|DateTimeOffset||
|name|String||
|registrant|[domainRegistrant](../resources/domainregistrant.md)||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

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

