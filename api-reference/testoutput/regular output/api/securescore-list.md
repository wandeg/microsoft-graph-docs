---
title: "List secureScores"
description: "List properties and relationships of the secureScore objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List secureScores

Namespace: microsoft.graph

List properties and relationships of the [secureScore](../resources/securescore.md) objects.

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
GET /Security/secureScores
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [secureScore](../resources/securescore.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/secureScores
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securescore)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1237

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.secureScore",
      "id": "532bd5c5-d5c5-532b-c5d5-2b53c5d52b53",
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
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
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

