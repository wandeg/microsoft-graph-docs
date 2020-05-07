---
title: "List ipSecurityProfiles"
description: "Get the ipSecurityProfiles from the ipSecurityProfiles navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List ipSecurityProfiles

Namespace: microsoft.graph

Get the ipSecurityProfiles from the ipSecurityProfiles navigation property.

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
GET /Security/ipSecurityProfiles
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

If successful, this method returns a `200 OK` response code and a collection of [ipSecurityProfile](../resources/ipsecurityprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ipsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/ipSecurityProfiles
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.ipsecurityprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ipSecurityProfile",
      "id": "ed147fa7-7fa7-ed14-a77f-14eda77f14ed",
      "activityGroupNames": [
        "String"
      ],
      "address": "String",
      "azureSubscriptionId": "String",
      "azureTenantId": "String",
      "countHits": "Integer",
      "countHosts": "Integer",
      "firstSeenDateTime": "String (timestamp)",
      "ipCategories": [
        {
          "@odata.type": "microsoft.graph.ipCategory"
        }
      ],
      "ipReferenceData": [
        {
          "@odata.type": "microsoft.graph.ipReferenceData"
        }
      ],
      "lastSeenDateTime": "String (timestamp)",
      "riskScore": "String",
      "tags": [
        "String"
      ],
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation"
      }
    }
  ]
}
```

