---
title: "Update cloudAppSecurityProfile"
description: "Update the properties of a cloudAppSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update cloudAppSecurityProfile

Namespace: microsoft.graph

Update the properties of a [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /Security/cloudAppSecurityProfiles/{cloudAppSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.

The following table shows the properties that are required when you create the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md).

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
|permissionsRequired|Enumeration| Possible values are: `unknown`, `anonymous`, `guest`, `user`, `administrator`, `system`, `unknownFutureValue`.|
|platform|String||
|policyName|String||
|publisher|String||
|riskScore|String||
|tags|String collection||
|type|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_cloudappsecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/cloudAppSecurityProfiles/{cloudAppSecurityProfileId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1047

{
  "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
  "id": "976cb8cc-b8cc-976c-ccb8-6c97ccb86c97",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
  "destinationServiceName": "Destination Service Name value",
  "isSigned": true,
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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

