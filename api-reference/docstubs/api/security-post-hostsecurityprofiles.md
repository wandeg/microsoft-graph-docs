---
title: "Create hostSecurityProfiles"
description: "Create a new hostSecurityProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create hostSecurityProfiles

Namespace: microsoft.graph

Create a new hostSecurityProfiles object.

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
POST /Security/hostSecurityProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [hostSecurityProfile](../resources/hostsecurityprofile.md) object.

The following table shows the properties that are required when you create the [hostSecurityProfile](../resources/hostsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|fqdn|String|**TODO: Add Description**|
|isAzureAdJoined|Boolean|**TODO: Add Description**|
|isAzureAdRegistered|Boolean|**TODO: Add Description**|
|isHybridAzureDomainJoined|Boolean|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|logonUsers|[logonUser](../resources/logonuser.md) collection|**TODO: Add Description**|
|netBiosName|String|**TODO: Add Description**|
|networkInterfaces|[networkInterface](../resources/networkinterface.md) collection|**TODO: Add Description**|
|os|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|parentHost|String|**TODO: Add Description**|
|relatedHostIds|String collection|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [hostSecurityProfile](../resources/hostsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_hostsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/hostSecurityProfiles
Content-Type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.hostSecurityProfile",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.hostsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

