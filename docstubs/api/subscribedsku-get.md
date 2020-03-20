---
title: "Get subscribedSku"
description: "Read properties and relationships of the subscribedSku object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get subscribedSku

Namespace: microsoft.graph

Read properties and relationships of the [subscribedSku](../resources/subscribedsku.md) object.

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
GET /subscribedSkus/{subscribedSkusId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}
-->
``` http
GET https://graph.microsoft.com/localtest/subscribedSkus/{subscribedSkusId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.subscribedSku",
    "id": "5bedb8bc-b8bc-5bed-bcb8-ed5bbcb8ed5b",
    "capabilityStatus": "Capability Status value",
    "consumedUnits": 13,
    "prepaidUnits": {
      "@odata.type": "microsoft.graph.licenseUnitsDetail",
      "enabled": 7,
      "suspended": 9,
      "warning": 7
    },
    "servicePlans": [
      {
        "@odata.type": "microsoft.graph.servicePlanInfo",
        "servicePlanId": "0181c468-c468-0181-68c4-810168c48101",
        "servicePlanName": "Service Plan Name value",
        "provisioningStatus": "Provisioning Status value",
        "appliesTo": "Applies To value"
      }
    ],
    "skuId": "2e1281ae-81ae-2e12-ae81-122eae81122e",
    "skuPartNumber": "Sku Part Number value",
    "appliesTo": "Applies To value"
  }
}
```

