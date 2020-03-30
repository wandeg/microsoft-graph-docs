---
title: "Add ipSecurityProfiles"
description: "Add ipSecurityProfiles by posting to the ipSecurityProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add ipSecurityProfiles

Namespace: microsoft.graph

Add ipSecurityProfiles by posting to the ipSecurityProfiles collection.

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
POST /Security/ipSecurityProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

The following table shows the properties that are required when you create the [ipSecurityProfile](../resources/ipsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection||
|address|String||
|azureSubscriptionId|String||
|azureTenantId|String||
|countHits|Int32||
|countHosts|Int32||
|firstSeenDateTime|DateTimeOffset||
|ipCategories|[ipCategory](../resources/ipcategory.md) collection||
|ipReferenceData|[ipReferenceData](../resources/ipreferencedata.md) collection||
|lastSeenDateTime|DateTimeOffset||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [ipSecurityProfile](../resources/ipsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_ipsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/ipSecurityProfiles
Content-type: application/json
Content-length: 1197

{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "address": "Address value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "countHits": 9,
  "countHosts": 10,
  "firstSeenDateTime": "2016-12-31T23:56:51.4119695+03:00",
  "ipCategories": [
    {
      "@odata.type": "microsoft.graph.ipCategory",
      "description": "Description value",
      "name": "Name value",
      "vendor": "Vendor value"
    }
  ],
  "ipReferenceData": [
    {
      "@odata.type": "microsoft.graph.ipReferenceData",
      "asn": 3,
      "city": "City value",
      "countryOrRegionCode": "Country Or Region Code value",
      "organization": "Organization value",
      "state": "State value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:01:49.1390274+03:00",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1246

{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "id": "e560b283-b283-e560-83b2-60e583b260e5",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "address": "Address value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "countHits": 9,
  "countHosts": 10,
  "firstSeenDateTime": "2016-12-31T23:56:51.4119695+03:00",
  "ipCategories": [
    {
      "@odata.type": "microsoft.graph.ipCategory",
      "description": "Description value",
      "name": "Name value",
      "vendor": "Vendor value"
    }
  ],
  "ipReferenceData": [
    {
      "@odata.type": "microsoft.graph.ipReferenceData",
      "asn": 3,
      "city": "City value",
      "countryOrRegionCode": "Country Or Region Code value",
      "organization": "Organization value",
      "state": "State value"
    }
  ],
  "lastSeenDateTime": "2017-01-01T00:01:49.1390274+03:00",
  "riskScore": "Risk Score value",
  "tags": [
    "Tags value"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value"
  }
}
```

