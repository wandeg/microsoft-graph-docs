---
title: "List cloudAppSecurityProfiles"
description: "Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List cloudAppSecurityProfiles

Namespace: microsoft.graph

Get the cloudAppSecurityProfiles from the cloudAppSecurityProfiles navigation property.

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
GET /Security/cloudAppSecurityProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [cloudAppSecurityProfile](../resources/cloudappsecurityprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_cloudappsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/cloudAppSecurityProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.cloudappsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudAppSecurityProfile",
      "id": "e1767c1a-7c1a-e176-1a7c-76e11a7c76e1",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "deploymentPackageUrl": "https://example.com/deploymentPackageUrl/",
      "destinationServiceName": "Destination Service Name value",
      "isSigned": true,
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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

