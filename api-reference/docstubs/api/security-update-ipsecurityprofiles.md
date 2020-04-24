---
title: "Update ipSecurityProfiles"
description: "Update the properties of an ipSecurityProfiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update ipSecurityProfiles

Namespace: microsoft.graph

Update the properties of an ipSecurityProfiles object.

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
PATCH /Security/ipSecurityProfiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

The following table shows the properties that are required when you create the [ipSecurityProfile](../resources/ipsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection|**TODO: Add Description**|
|address|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|countHits|Int32|**TODO: Add Description**|
|countHosts|Int32|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|ipCategories|[ipCategory](../resources/ipcategory.md) collection|**TODO: Add Description**|
|ipReferenceData|[ipReferenceData](../resources/ipreferencedata.md) collection|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [ipSecurityProfile](../resources/ipsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ipsecurityprofiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/ipSecurityProfiles
Content-Type: application/json
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
  "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
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
  "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "id": "70392a92-2a92-7039-922a-3970922a3970",
  "activityGroupNames": [
    "Activity Group Names value"
  ],
  "address": "Address value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "countHits": 9,
  "countHosts": 10,
  "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
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
  "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
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

