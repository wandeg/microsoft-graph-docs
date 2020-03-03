---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create subscribedSku

Create a new [subscribedSku](../resources/subscribedsku.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /subscribedSkus
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the subscribedSku object.

The following table shows the properties that are required when you create the subscribedSku.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|capabilityStatus|String||
|consumedUnits|Int32||
|prepaidUnits|[licenseUnitsDetail](../resources/licenseUnitsDetail.md)||
|servicePlans|[servicePlanInfo](../resources/servicePlanInfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||
|appliesTo|String||



## Response
If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/subscribedSkus
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
      "servicePlanId": "f778b540-b540-f778-40b5-78f740b578f7",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "57435096-5096-5743-9650-435796504357",
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
  "id": "beed23ec-23ec-beed-ec23-edbeec23edbe",
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
      "servicePlanId": "f778b540-b540-f778-40b5-78f740b578f7",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "57435096-5096-5743-9650-435796504357",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

