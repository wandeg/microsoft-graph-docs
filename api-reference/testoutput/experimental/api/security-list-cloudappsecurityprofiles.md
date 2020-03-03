---
title: "List cloudAppSecurityProfiles"
description: "Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List cloudAppSecurityProfiles

Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property.

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
GET /Security/cloudAppSecurityProfiles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_cloudappsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/Security/cloudAppSecurityProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.cloudappsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
      "id": "053c36a0-36a0-053c-a036-3c05a0363c05",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
      "destinationServiceName": "Destination Service Name value",
      "isSigned": true,
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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
  ]
}
```

