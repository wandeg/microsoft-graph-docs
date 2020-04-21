---
title: "List secureScores"
description: "Get the secureScores from the secureScores navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List secureScores

Namespace: microsoft.graph

Get the secureScores from the secureScores navigation property.

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
GET /Security/secureScores
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
If successful, this method returns a `200 OK` response code and a collection of [secureScore](../resources/securescore.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/secureScores
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securescore)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.secureScore",
      "id": "24050234-0234-2405-3402-052434020524",
      "activeUserCount": 15,
      "averageComparativeScores": [
        {
          "@odata.type": "microsoft.graph.averageComparativeScore",
          "averageScore": "Double",
          "basis": "Basis value"
        }
      ],
      "azureTenantId": "Azure Tenant Id value",
      "controlScores": [
        {
          "@odata.type": "microsoft.graph.controlScore",
          "controlCategory": "Control Category value",
          "controlName": "Control Name value",
          "description": "Description value",
          "score": "Double"
        }
      ],
      "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
      "currentScore": "Double",
      "enabledServices": [
        "Enabled Services value"
      ],
      "licensedUserCount": 1,
      "maxScore": "Double",
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

