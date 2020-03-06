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
|[Get cloudAppSecurityProfile](../api/cloudappsecurityprofile-get.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Read properties and relationships of the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.|
|[Update cloudAppSecurityProfile](../api/cloudappsecurityprofile-update.md)|[cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md)|Update the properties of a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.|

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

## JSON representation
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

