---
title: "Get hostSecurityProfile"
description: "Read the properties and relationships of a hostSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get hostSecurityProfile

Namespace: microsoft.graph

Read the properties and relationships of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.

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
GET /Security/hostSecurityProfiles/{hostSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and a [hostSecurityProfile](../resources/hostsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_hostsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/hostSecurityProfiles/{hostSecurityProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.hostSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.hostSecurityProfile",
    "id": "93e56cd1-6cd1-93e5-d16c-e593d16ce593",
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
    "fqdn": "Fqdn value",
    "isAzureAdJoined": true,
    "isAzureAdRegistered": true,
    "isHybridAzureDomainJoined": true,
    "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
    "logonUsers": [
      {
        "@odata.type": "microsoft.graph.logonUser",
        "accountDomain": "Account Domain value",
        "accountName": "Account Name value",
        "accountType": "String",
        "logonId": "Logon Id value",
        "logonTypes": [
          "String"
        ]
      }
    ],
    "netBiosName": "Net Bios Name value",
    "networkInterfaces": [
      {
        "@odata.type": "microsoft.graph.networkInterface",
        "description": "Description value",
        "ipV4Address": "Ip V4Address value",
        "ipV6Address": "Ip V6Address value",
        "localIpV6Address": "Local Ip V6Address value",
        "macAddress": "Mac Address value"
      }
    ],
    "os": "Os value",
    "osVersion": "Os Version value",
    "parentHost": "Parent Host value",
    "relatedHostIds": [
      "Related Host Ids value"
    ],
    "riskScore": "Risk Score value",
    "tags": [
      "Tags value"
    ],
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

