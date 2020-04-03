---
title: "Update domainSecurityProfile"
description: "Update the properties of a domainSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domainSecurityProfile

Namespace: microsoft.graph

Update the properties of a [domainSecurityProfile](../resources/domainsecurityprofile.md) object.

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
PATCH /Security/domainSecurityProfiles/{domainSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [domainSecurityProfile](../resources/domainsecurityprofile.md) object.

The following table shows the properties that are required when you create the [domainSecurityProfile](../resources/domainsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection||
|azureSubscriptionId|String||
|azureTenantId|String||
|countHits|Int32||
|countInOrg|Int32||
|domainCategories|[reputationCategory](../resources/reputationcategory.md) collection||
|domainRegisteredDateTime|DateTimeOffset||
|firstSeenDateTime|DateTimeOffset||
|lastSeenDateTime|DateTimeOffset||
|name|String||
|registrant|[domainRegistrant](../resources/domainregistrant.md)||
|riskScore|String||
|tags|String collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [domainSecurityProfile](../resources/domainsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domainsecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/domainSecurityProfiles/{domainSecurityProfileId}
Content-type: application/json
Content-length: 1197

{
  "@odata.type": "#microsoft.graph.domainSecurityProfile",
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
  "domainRegisteredDateTime": "2016-12-31T23:58:33.571195+00:00",
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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
Content-Length: 1246

{
  "@odata.type": "#microsoft.graph.domainSecurityProfile",
  "id": "cece08b5-08b5-cece-b508-ceceb508cece",
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
  "domainRegisteredDateTime": "2016-12-31T23:58:33.571195+00:00",
  "firstSeenDateTime": "2016-12-31T23:57:13.529911+00:00",
  "lastSeenDateTime": "2016-12-31T23:58:33.6279063+00:00",
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
```

