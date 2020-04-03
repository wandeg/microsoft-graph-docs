---
title: "Update hostSecurityProfile"
description: "Update the properties of a hostSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update hostSecurityProfile

Namespace: microsoft.graph

Update the properties of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.

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
PATCH /Security/hostSecurityProfiles/{hostSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [hostSecurityProfile](../resources/hostsecurityprofile.md) object.

The following table shows the properties that are required when you create the [hostSecurityProfile](../resources/hostsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|azureSubscriptionId|String||
|azureTenantId|String||
|firstSeenDateTime|DateTimeOffset||
|fqdn|String||
|isAzureAdJoined|Boolean||
|isAzureAdRegistered|Boolean||
|isHybridAzureDomainJoined|Boolean||
|lastSeenDateTime|DateTimeOffset||
|logonUsers|[logonUser](../resources/logonuser.md) collection||
|netBiosName|String||
|networkInterfaces|[networkInterface](../resources/networkinterface.md) collection||
|os|String||
|osVersion|String||
|parentHost|String||
|relatedHostIds|String collection||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [hostSecurityProfile](../resources/hostsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_hostsecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/hostSecurityProfiles/{hostSecurityProfileId}
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "fqdn": "Fqdn value",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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
Content-Length: 1608

{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "id": "b4e4a1ee-a1ee-b4e4-eea1-e4b4eea1e4b4",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "fqdn": "Fqdn value",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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
```

