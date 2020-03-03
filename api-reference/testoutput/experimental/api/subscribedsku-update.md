---
title: "Update subscribedSku"
description: "Update the properties of a subscribedSku object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update subscribedSku

Namespace: microsoft.graph

Update the properties of a [subscribedSku](../resources/subscribedsku.md) object.

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
PATCH /subscribedSkus/{subscribedSkusId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
If successful, this method returns a `200 OK` response code and an updated [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_subscribedsku"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/subscribedSkus/{subscribedSkusId}
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
      "servicePlanId": "2f12abad-abad-2f12-adab-122fadab122f",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "766f47e4-47e4-766f-e447-6f76e4476f76",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 766

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "id": "d7eb8ca3-8ca3-d7eb-a38c-ebd7a38cebd7",
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
      "servicePlanId": "2f12abad-abad-2f12-adab-122fadab122f",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "766f47e4-47e4-766f-e447-6f76e4476f76",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

