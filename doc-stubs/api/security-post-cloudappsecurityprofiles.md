---
title: "Create cloudAppSecurityProfiles"
description: "Create a new cloudAppSecurityProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create cloudAppSecurityProfiles

Namespace: microsoft.graph

Create a new cloudAppSecurityProfiles object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /Security/cloudAppSecurityProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.

The following table shows the properties that are required when you create the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentPackageUrl|String|**TODO: Add Description**|
|destinationServiceName|String|**TODO: Add Description**|
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



## Response

If successful, this method returns a `201 Created` response code and a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_cloudappsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/cloudAppSecurityProfiles
Content-Type: application/json
Content-length: 569

{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "deploymentPackageUrl": "String",
  "destinationServiceName": "String",
  "isSigned": "Boolean",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudappsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "id": "06f09e41-9e41-06f0-419e-f006419ef006",
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

