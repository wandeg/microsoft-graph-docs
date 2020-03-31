---
title: "Update ipSecurityProfile"
description: "Update the properties of a ipSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update ipSecurityProfile

Namespace: microsoft.graph

Update the properties of a [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

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
PATCH /Security/ipSecurityProfiles/{ipSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [ipSecurityProfile](../resources/ipsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_ipsecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/ipSecurityProfiles/{ipSecurityProfileId}
Content-type: application/json
Content-length: 1196

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
  "firstSeenDateTime": "2017-01-01T00:01:22.395975+03:00",
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
  "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "id": "2b2687a4-87a4-2b26-a487-262ba487262b",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "address": "Address value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "countHits": 9,
  "countHosts": 10,
  "firstSeenDateTime": "2017-01-01T00:01:22.395975+03:00",
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
  "lastSeenDateTime": "2017-01-01T00:01:35.9495977+03:00",
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

