---
title: "Add cloudAppSecurityProfiles"
description: "Add cloudAppSecurityProfiles by posting to the cloudAppSecurityProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add cloudAppSecurityProfiles

Add cloudAppSecurityProfiles by posting to the cloudAppSecurityProfiles collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /Security/cloudAppSecurityProfiles/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the cloudAppSecurityProfile object.

The following table shows the properties that are required when you create the cloudAppSecurityProfile.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|azureSubscriptionId|String||
|azureTenantId|String||
|createdDateTime|DateTimeOffset||
|deploymentPackageUrl|String||
|destinationServiceName|String||
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
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_cloudappsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/Security/cloudAppSecurityProfiles
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudappsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1047

{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "id": "053c36a0-36a0-053c-a036-3c05a0363c05",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
  "destinationServiceName": "Destination Service Name value",
  "isSigned": true,
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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

