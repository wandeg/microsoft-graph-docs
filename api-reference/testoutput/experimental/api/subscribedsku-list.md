---
title: "List subscribedSkus"
description: "List properties and relationships of the subscribedSku objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List subscribedSkus

Namespace: microsoft.graph

List properties and relationships of the [subscribedSku](../resources/subscribedsku.md) objects.

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
GET /subscribedSkus
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
If successful, this method returns a `200 OK` response code and a collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}
-->
``` http
GET https://graph.microsoft.com/localtest/subscribedSkus
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.subscribedsku)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 887

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.subscribedSku",
      "id": "6914adcc-adcc-6914-ccad-1469ccad1469",
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
          "servicePlanId": "430099a8-99a8-4300-a899-0043a8990043",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "25470e04-0e04-2547-040e-4725040e4725",
      "skuPartNumber": "Sku Part Number value",
      "appliesTo": "Applies To value"
    }
  ]
}
```

