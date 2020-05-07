---
title: "cloudAppSecurityProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudAppSecurityProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentPackageUrl|String|**TODO: Add Description**|
|destinationServiceName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isSigned|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|manifest|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|permissionsRequired|applicationPermissionsRequired|**TODO: Add Description**. Possible values are: `unknown`, `anonymous`, `guest`, `user`, `administrator`, `system`, `unknownFutureValue`.|
|platform|String|**TODO: Add Description**|
|policyName|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "isSigned": "Boolean",
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

