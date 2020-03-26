---
title: "Add licenseDetails"
description: "Add licenseDetails by posting to the licenseDetails collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add licenseDetails

Namespace: microsoft.graph

Add licenseDetails by posting to the licenseDetails collection.

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
POST /me/licenseDetails/$ref
POST /users/{usersId}/licenseDetails/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [licenseDetails](../resources/licensedetails.md) object.

The following table shows the properties that are required when you create the [licenseDetails](../resources/licensedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||



## Response
If successful, this method returns a `201 Created` response code and a [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_licensedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/licenseDetails
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "3140b495-b495-3140-95b4-403195b44031",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "74a48260-8260-74a4-6082-a4746082a474",
  "skuPartNumber": "Sku Part Number value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licensedetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 514

{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "622ee6c3-e6c3-622e-c3e6-2e62c3e62e62",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "3140b495-b495-3140-95b4-403195b44031",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "74a48260-8260-74a4-6082-a4746082a474",
  "skuPartNumber": "Sku Part Number value"
}
```

