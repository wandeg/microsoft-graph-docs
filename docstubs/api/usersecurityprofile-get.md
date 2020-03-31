---
title: "Get userSecurityProfile"
description: "Read properties and relationships of the userSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userSecurityProfile

Namespace: microsoft.graph

Read properties and relationships of the [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
GET /Security/userSecurityProfiles/{userSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usersecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/userSecurityProfiles/{userSecurityProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1175

{
  "value": {
    "@odata.type": "#microsoft.graph.userSecurityProfile",
    "id": "e0f45d37-5d37-e0f4-375d-f4e0375df4e0",
    "accounts": [
      {
        "@odata.type": "microsoft.graph.userAccount",
        "displayName": "Display Name value",
        "lastSeenDateTime": "2016-12-31T23:58:01.4389058+03:00",
        "riskScore": "Risk Score value",
        "service": "Service value",
        "signinName": "Signin Name value",
        "status": "String"
      }
    ],
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
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
}
```

