---
title: "List ipSecurityProfiles"
description: "Get the ipSecurityProfiles from the ipSecurityProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List ipSecurityProfiles

Namespace: microsoft.graph

Get the ipSecurityProfiles from the ipSecurityProfiles navigation property.

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
GET /Security/ipSecurityProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [ipSecurityProfile](../resources/ipsecurityprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_ipsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/ipSecurityProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.ipsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ipSecurityProfile",
      "id": "edfd3c86-3c86-edfd-863c-fded863cfded",
      "activityGroupNames": [
        "Activity Group Names value"
      ],
      "address": "Address value",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "countHits": 9,
      "countHosts": 10,
      "firstSeenDateTime": "2016-12-31T23:58:40.1273666+03:00",
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
      "lastSeenDateTime": "2016-12-31T23:58:01.4389058+03:00",
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
  ]
}
```

