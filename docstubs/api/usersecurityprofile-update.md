---
title: "Update userSecurityProfile"
description: "Update the properties of a userSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userSecurityProfile

Namespace: microsoft.graph

Update the properties of a [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
PATCH /Security/userSecurityProfiles/{userSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userSecurityProfile](../resources/usersecurityprofile.md) object.

The following table shows the properties that are required when you create the [userSecurityProfile](../resources/usersecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accounts|[userAccount](../resources/useraccount.md) collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|createdDateTime|DateTimeOffset||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||
|riskScore|String||
|tags|String collection||
|userPrincipalName|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_usersecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/userSecurityProfiles/{userSecurityProfileId}
Content-type: application/json
Content-length: 924

{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
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
  "id": "5f0446e2-46e2-5f04-e246-045fe246045f",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
      "riskScore": "Risk Score value",
      "service": "Service value",
      "signinName": "Signin Name value",
      "status": "String"
    }
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
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

