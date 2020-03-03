---
title: "Create userSecurityProfile"
description: "Create a new userSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create userSecurityProfile

Namespace: microsoft.graph

Create a new [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
POST /Security/userSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_usersecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/Security/userSecurityProfiles
Content-type: application/json
Content-length: 923

{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2016-12-31T23:59:38.861959+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.usersecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1094

{
  "@odata.type": "#microsoft.graph.userSecurityProfile",
  "id": "c8b65270-5270-c8b6-7052-b6c87052b6c8",
  "accounts": [
    {
      "@odata.type": "microsoft.graph.userAccount",
      "displayName": "Display Name value",
      "lastSeenDateTime": "2016-12-31T23:59:38.861959+03:00",
      "riskScore": "Risk Score value",
      "service": "Service value",
      "signinName": "Signin Name value",
      "status": "String"
    }
  ],
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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

