---
title: "Add domainSecurityProfiles"
description: "Add domainSecurityProfiles by posting to the domainSecurityProfiles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add domainSecurityProfiles

Namespace: microsoft.graph

Add domainSecurityProfiles by posting to the domainSecurityProfiles collection.

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
POST /Security/domainSecurityProfiles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [domainSecurityProfile](../resources/domainsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domainsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/domainSecurityProfiles
Content-type: application/json
Content-length: 1199

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
  "domainRegisteredDateTime": "2017-01-01T00:03:12.2448626+03:00",
  "firstSeenDateTime": "2017-01-01T00:00:12.1297001+03:00",
  "lastSeenDateTime": "2017-01-01T00:01:06.2277213+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.domainsecurityprofile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.domainSecurityProfile",
  "id": "838f04f4-04f4-838f-f404-8f83f4048f83",
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
  "domainRegisteredDateTime": "2017-01-01T00:03:12.2448626+03:00",
  "firstSeenDateTime": "2017-01-01T00:00:12.1297001+03:00",
  "lastSeenDateTime": "2017-01-01T00:01:06.2277213+03:00",
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

