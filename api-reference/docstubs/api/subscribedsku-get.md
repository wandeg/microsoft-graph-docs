---
title: "Get subscribedSku"
description: "Read the properties and relationships of a subscribedSku object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get subscribedSku

Namespace: microsoft.graph

Read the properties and relationships of a [subscribedSku](../resources/subscribedsku.md) object.

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
GET /subscribedSkus/{subscribedSkusId}
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
If successful, this method returns a `200 OK` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}
-->
``` http
GET https://graph.microsoft.com/beta/subscribedSkus/{subscribedSkusId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.subscribedSku",
    "id": "33c90cb5-0cb5-33c9-b50c-c933b50cc933",
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
        "servicePlanId": "ba5fb184-b184-ba5f-84b1-5fba84b15fba",
        "servicePlanName": "Service Plan Name value",
        "provisioningStatus": "Provisioning Status value",
        "appliesTo": "Applies To value"
      }
    ],
    "skuId": "747ec031-c031-747e-31c0-7e7431c07e74",
    "skuPartNumber": "Sku Part Number value",
    "appliesTo": "Applies To value"
  }
}
```

