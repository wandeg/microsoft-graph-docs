---
title: "Update cloudAppSecurityProfiles"
description: "Update the properties of a cloudAppSecurityProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cloudAppSecurityProfiles

Namespace: microsoft.graph

Update the properties of a cloudAppSecurityProfiles object.

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
PATCH /Security/cloudAppSecurityProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cloudappsecurityprofiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/cloudAppSecurityProfiles
Content-Type: application/json
Content-length: 875

{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
  "destinationServiceName": "Destination Service Name value",
  "isSigned": true,
  "manifest": "Manifest value",
  "name": "Name value",
  "permissionsRequired": "String",
  "platform": "Platform value",
  "policyName": "Policy Name value",
  "publisher": "Publisher value",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "type": "Type value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "id": "e1767c1a-7c1a-e176-1a7c-76e11a7c76e1",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
  "destinationServiceName": "Destination Service Name value",
  "isSigned": true,
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "manifest": "Manifest value",
  "name": "Name value",
  "permissionsRequired": "String",
  "platform": "Platform value",
  "policyName": "Policy Name value",
  "publisher": "Publisher value",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "type": "Type value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

