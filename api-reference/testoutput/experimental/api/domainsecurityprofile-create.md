---
title: "Create domainSecurityProfile"
description: "Create a new domainSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domainSecurityProfile

Namespace: microsoft.graph

Create a new [domainSecurityProfile](../resources/domainsecurityprofile.md) object.

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
POST /Security/domainSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domainsecurityprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/Security/domainSecurityProfiles
Content-type: application/json
Content-length: 1198

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
Content-Length: 1247

{
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
```

