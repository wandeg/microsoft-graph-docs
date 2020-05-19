---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create subscribedSku

Namespace: microsoft.graph

Create a new [subscribedSku](../resources/subscribedsku.md) object.

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
POST /subscribedSkus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [subscribedSku](../resources/subscribedsku.md) object.

The following table shows the properties that are required when you create the [subscribedSku](../resources/subscribedsku.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|capabilityStatus|String|**TODO: Add Description**|
|consumedUnits|Int32|**TODO: Add Description**|
|prepaidUnits|[licenseUnitsDetail](../resources/licenseunitsdetail.md)|**TODO: Add Description**|
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|
|appliesTo|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/subscribedSkus
Content-Type: application/json
Content-length: 376

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedsku"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "id": "a9ff9bb3-9bb3-a9ff-b39b-ffa9b39bffa9",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```

