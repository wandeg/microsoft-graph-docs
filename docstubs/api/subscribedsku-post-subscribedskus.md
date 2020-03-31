---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create subscribedSku

Namespace: microsoft.graph

Create a new [subscribedSku](../resources/subscribedsku.md) object.

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
POST /subscribedSkus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [subscribedSku](../resources/subscribedsku.md) object.

The following table shows the properties that are required when you create the [subscribedSku](../resources/subscribedsku.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|capabilityStatus|String||
|consumedUnits|Int32||
|prepaidUnits|[licenseUnitsDetail](../resources/licenseunitsdetail.md)||
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||
|appliesTo|String||



## Response
If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/beta/subscribedSkus
Content-type: application/json
Content-length: 717

{
  "@odata.type": "#microsoft.graph.subscribedSku",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedsku"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 766

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
```

