---
title: "Get cloudAppSecurityProfile"
description: "Read properties and relationships of the cloudAppSecurityProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get cloudAppSecurityProfile

Namespace: microsoft.graph

Read properties and relationships of the [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object.

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
GET /Security/cloudAppSecurityProfiles/{cloudAppSecurityProfileId}
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
If successful, this method returns a `200 OK` response code and [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_cloudappsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/cloudAppSecurityProfiles/{cloudAppSecurityProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudAppSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1120

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
    "id": "ee25135b-135b-ee25-5b13-25ee5b1325ee",
    "azureSubscriptionId": "Azure Subscription Id value",
    "azureTenantId": "Azure Tenant Id value",
    "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
    "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
    "destinationServiceName": "Destination Service Name value",
    "isSigned": true,
    "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00",
    "manifest": "Manifest value",
    "name": "Name value",
    "permissionsRequired": "String",
    "platform": "Platform value",
    "policyName": "Policy Name value",
    "publisher": "Publisher value",
    "riskScore": "Risk Score value",
    "tags": [
      "Tags value"
    ],
    "type": "Type value",
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation",
      "provider": "Provider value",
      "providerVersion": "Provider Version value",
      "subProvider": "Sub Provider value",
      "vendor": "Vendor value"
    }
  }
}
```

