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
|Name|Description|
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
GET https://graph.microsoft.com/beta/subscribedSkus
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
      "id": "af845038-5038-af84-3850-84af385084af",
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
          "servicePlanId": "4a8ded43-ed43-4a8d-43ed-8d4a43ed8d4a",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "728dbca0-bca0-728d-a0bc-8d72a0bc8d72",
      "skuPartNumber": "Sku Part Number value",
      "appliesTo": "Applies To value"
    }
  ]
}
```

