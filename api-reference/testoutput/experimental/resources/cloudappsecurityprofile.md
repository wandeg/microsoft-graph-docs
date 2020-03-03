---
title: "cloudAppSecurityProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cloudAppSecurityProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List cloudAppSecurityProfiles](../api/cloudappsecurityprofile-list.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection|List properties and relationships of the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) objects.|
|[Get cloudAppSecurityProfile](../api/cloudappsecurityprofile-get.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Read properties and relationships of the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.|
|[Create cloudAppSecurityProfile](../api/cloudappsecurityprofile-create.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Create a new [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.|
|[Delete cloudAppSecurityProfile](../api/cloudappsecurityprofile-delete.md)|None|Deletes a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md).|
|[Update cloudAppSecurityProfile](../api/cloudappsecurityprofile-update.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Update the properties of a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.|
|[List cloudAppSecurityProfiles](../api/security-list-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) collection|Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property.|
|[Add cloudAppSecurityProfiles](../api/security-post-cloudappsecurityprofiles.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Add cloudAppSecurityProfiles by posting to the cloudAppSecurityProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureSubscriptionId|String||
|azureTenantId|String||
|createdDateTime|DateTimeOffset||
|deploymentPackageUrl|String||
|destinationServiceName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isSigned|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|manifest|String||
|name|String||
|permissionsRequired|Enumeration|. Possible values are: `unknown`, `anonymous`, `guest`, `user`, `administrator`, `system`, `unknownFutureValue`.|
|platform|String||
|policyName|String||
|publisher|String||
|riskScore|String||
|tags|String collection||
|type|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudAppSecurityProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "id": "String (identifier)",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "createdDateTime": "String (timestamp)",
  "deploymentPackageUrl": "String",
  "destinationServiceName": "String",
  "isSigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "manifest": "String",
  "name": "String",
  "permissionsRequired": "String",
  "platform": "String",
  "policyName": "String",
  "publisher": "String",
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "type": "String",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

