---
title: "Get domainSecurityProfile"
description: "Read properties and relationships of the domainSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domainSecurityProfile

Namespace: microsoft.graph

Read properties and relationships of the [domainSecurityProfile](../resources/domainsecurityprofile.md) object.

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
GET /Security/domainSecurityProfiles/{domainSecurityProfileId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [domainSecurityProfile](../resources/domainsecurityprofile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domainsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/domainSecurityProfiles/{domainSecurityProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1340

{
  "value": {
    "@odata.type": "#microsoft.graph.domainSecurityProfile",
    "id": "2db8f0b7-f0b7-2db8-b7f0-b82db7f0b82d",
    "activityGroupNames": [
      "Activity Group Names value"
    ],
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "countHits": 9,
    "countInOrg": 10,
    "domainCategories": [
      {
        "@odata.type": "microsoft.graph.reputationCategory",
        "description": "Description value",
        "name": "Name value",
        "vendor": "Vendor value"
      }
    ],
    "domainRegisteredDateTime": "2017-01-01T00:00:56.6394557+03:00",
    "firstSeenDateTime": "2016-12-31T23:57:18.6460025+03:00",
    "lastSeenDateTime": "2016-12-31T23:59:38.861959+03:00",
    "name": "Name value",
    "registrant": {
      "@odata.type": "microsoft.graph.domainRegistrant",
      "countryOrRegionCode": "Country Or Region Code value",
      "organization": "Organization value",
      "url": "Url value"
    },
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

