---
title: "Update licenseDetails"
description: "Update the properties of a licenseDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update licenseDetails

Namespace: microsoft.graph

Update the properties of a licenseDetails object.

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
PATCH /servicePrincipals/{servicePrincipalsId}/licenseDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [licenseDetails](../resources/licensedetails.md) object.

The following table shows the properties that are required when you create the [licenseDetails](../resources/licensedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_licensedetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/licenseDetails
Content-Type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.licenseDetails",
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
  "skuPartNumber": "Sku Part Number value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "2fa919af-19af-2fa9-af19-a92faf19a92f",
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
  "skuPartNumber": "Sku Part Number value"
}
```

