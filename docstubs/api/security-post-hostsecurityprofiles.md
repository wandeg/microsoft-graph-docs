---
title: "Add hostSecurityProfiles"
description: "Add hostSecurityProfiles by posting to the hostSecurityProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add hostSecurityProfiles

Namespace: microsoft.graph

Add hostSecurityProfiles by posting to the hostSecurityProfiles collection.

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
POST /Security/hostSecurityProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [hostSecurityProfile](../resources/hostsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_hostsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/hostSecurityProfiles
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "firstSeenDateTime": "2017-01-01T00:01:22.395975+03:00",
  "fqdn": "Fqdn value",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.hostsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1608

{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
  "id": "75df1e24-1e24-75df-241e-df75241edf75",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "firstSeenDateTime": "2017-01-01T00:01:22.395975+03:00",
  "fqdn": "Fqdn value",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
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

