---
title: "Get userSecurityProfile"
description: "Read the properties and relationships of a userSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get userSecurityProfile

Namespace: microsoft.graph

Read the properties and relationships of a [userSecurityProfile](../resources/usersecurityprofile.md) object.

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
GET /Security/userSecurityProfiles/{userSecurityProfileId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [userSecurityProfile](../resources/usersecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_usersecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/userSecurityProfiles/{userSecurityProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.userSecurityProfile",
    "id": "8418c686-c686-8418-86c6-188486c61884",
    "accounts": [
      {
        "@odata.type": "microsoft.graph.userAccount",
        "displayName": "Display Name value",
        "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
        "riskScore": "Risk Score value",
        "service": "Service value",
        "signinName": "Signin Name value",
        "status": "String"
      }
    ],
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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

