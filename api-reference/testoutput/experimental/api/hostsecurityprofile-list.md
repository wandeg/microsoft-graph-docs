---
title: "List hostSecurityProfiles"
description: "List properties and relationships of the hostSecurityProfile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List hostSecurityProfiles

Namespace: microsoft.graph

List properties and relationships of the [hostSecurityProfile](../resources/hostsecurityprofile.md) objects.

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
GET /Security/hostSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [hostSecurityProfile](../resources/hostsecurityprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_hostsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/hostSecurityProfiles
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
Content-Length: 1841

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.hostSecurityProfile",
      "id": "ca4bc022-c022-ca4b-22c0-4bca22c04bca",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "firstSeenDateTime": "2016-12-31T23:57:18.6460025+03:00",
      "fqdn": "Fqdn value",
      "isAzureAdJoined": true,
      "isAzureAdRegistered": true,
      "isHybridAzureDomainJoined": true,
      "lastSeenDateTime": "2016-12-31T23:59:38.861959+03:00",
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

