---
title: "Create licenseDetails"
description: "Create a new licenseDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create licenseDetails

Namespace: microsoft.graph

Create a new [licenseDetails](../resources/licensedetails.md) object.

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
POST /me/licenseDetails
POST /users/{usersId}/licenseDetails
POST /servicePrincipals/{servicePrincipalsId}/licenseDetails
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_licensedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/licenseDetails
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.licenseDetails",
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
  "id": "5dfe710e-710e-5dfe-0e71-fe5d0e71fe5d",
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
  "skuPartNumber": "Sku Part Number value"
}
```

