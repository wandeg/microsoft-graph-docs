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
|Authorization|Bearer {token}. Required.|

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
      "id": "06f09e41-9e41-06f0-419e-f006419ef006",
      "azureSubscriptionId": "String",
      "azureTenantId": "String",
      "createdDateTime": "String (timestamp)",
      "deploymentPackageUrl": "String",
      "destinationServiceName": "String",
      "isSigned": "Boolean",
      "lastModifiedDateTime": "String (timestamp)",
      "manifest": "String",
      "name": "String",
      "permissionsRequired": "String",
      "platform": "String",
      "policyName": "String",
      "publisher": "String",
      "riskScore": "String",
      "tags": [
        "String"
      ],
      "type": "String",
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation"
      }
    }
  ]
}
```

