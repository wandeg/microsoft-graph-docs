---
title: "List userSecurityProfiles"
description: "Get the userSecurityProfiles from the userSecurityProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userSecurityProfiles

Namespace: microsoft.graph

Get the userSecurityProfiles from the userSecurityProfiles navigation property.

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
GET /Security/userSecurityProfiles
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userSecurityProfile](../resources/usersecurityprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usersecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/userSecurityProfiles
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
      "id": "409bf3a9-f3a9-409b-a9f3-9b40a9f39b40",
      "accounts": [
        {
          "@odata.type": "microsoft.graph.userAccount",
          "displayName": "Display Name value",
          "lastSeenDateTime": "2017-01-01T00:02:45.4710492+03:00",
          "riskScore": "Risk Score value",
          "service": "Service value",
          "signinName": "Signin Name value",
          "status": "String"
        }
      ],
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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

