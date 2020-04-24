---
title: "Get domainSecurityProfile"
description: "Read the properties and relationships of a domainSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get domainSecurityProfile

Namespace: microsoft.graph

Read the properties and relationships of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.

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
GET /Security/domainSecurityProfiles/{domainSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and a [domainSecurityProfile](../resources/domainsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domainsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/domainSecurityProfiles/{domainSecurityProfileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.domainSecurityProfile",
    "id": "cd5b9322-9322-cd5b-2293-5bcd22935bcd",
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
    "domainRegisteredDateTime": "2017-01-01T00:03:19.3779468+03:00",
    "firstSeenDateTime": "2016-12-31T23:56:24.2596319+03:00",
    "lastSeenDateTime": "2017-01-01T00:02:18.945458+03:00",
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

