---
title: "List userSecurityProfiles"
description: "Get the userSecurityProfiles from the userSecurityProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userSecurityProfiles

Get the userSecurityProfiles from the userSecurityProfiles navigation property.

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
GET /Security/userSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userSecurityProfile](../resources/usersecurityprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usersecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/Security/userSecurityProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.usersecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1249

{
  "value": [
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
  ]
}
```

