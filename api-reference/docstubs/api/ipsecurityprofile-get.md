---
title: "Get ipSecurityProfile"
description: "Read the properties and relationships of an ipSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get ipSecurityProfile

Namespace: microsoft.graph

Read the properties and relationships of an [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

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
GET /Security/ipSecurityProfiles/{ipSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and an [ipSecurityProfile](../resources/ipsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ipsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/ipSecurityProfiles/{ipSecurityProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

