---
title: "List hostSecurityProfiles"
description: "Get the hostSecurityProfiles from the hostSecurityProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List hostSecurityProfiles

Namespace: microsoft.graph

Get the hostSecurityProfiles from the hostSecurityProfiles navigation property.

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
GET /Security/hostSecurityProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [hostSecurityProfile](../resources/hostsecurityprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_hostsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/hostSecurityProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.hostsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.hostSecurityProfile",
      "id": "a2677e0b-7e0b-a267-0b7e-67a20b7e67a2",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "firstSeenDateTime": "2017-01-01T00:02:25.6939099+00:00",
      "fqdn": "Fqdn value",
      "isAzureAdJoined": true,
      "isAzureAdRegistered": true,
      "isHybridAzureDomainJoined": true,
      "lastSeenDateTime": "2017-01-01T00:01:32.8955884+00:00",
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
  ]
}
```

