---
title: "Update userSecurityProfile"
description: "Update the properties of a userSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userSecurityProfile

Update the properties of a [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
PATCH /Security/userSecurityProfiles/{userSecurityProfileId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [userSecurityProfile](../resources/userSecurityProfile.md) object.

The following table shows the properties that are required when you create the [userSecurityProfile](../resources/usersecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accounts|[userAccount](../resources/userAccount.md) collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|createdDateTime|DateTimeOffset||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||
|riskScore|String||
|tags|String collection||
|userPrincipalName|String||
|vendorInformation|[securityVendorInformation](../resources/securityVendorInformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_usersecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/Security/userSecurityProfiles/{userSecurityProfileId}
Content-type: application/json
Content-length: 924

{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2016-12-31T23:58:05.5931807+03:00",
      "riskScore": "Risk Score value",
      "service": "Service value",
      "signinName": "Signin Name value",
      "status": "String"
    }
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "displayName": "Display Name value",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "userPrincipalName": "User Principal Name value",
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
Content-Length: 1096

{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "id": "e9107a0b-7a0b-e910-0b7a-10e90b7a10e9",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2016-12-31T23:58:05.5931807+03:00",
      "riskScore": "Risk Score value",
      "service": "Service value",
      "signinName": "Signin Name value",
      "status": "String"
    }
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "userPrincipalName": "User Principal Name value",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

