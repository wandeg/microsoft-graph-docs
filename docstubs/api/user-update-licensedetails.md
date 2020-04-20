---
title: "Update licenseDetails"
description: "Update the properties of a licenseDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
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
PATCH /me/licenseDetails
PATCH /users/{usersId}/licenseDetails
PATCH /invitations/{invitationsId}/invitedUser/licenseDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [licenseDetails](../resources/licensedetails.md) object.

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
PATCH https://graph.microsoft.com/beta/me/licenseDetails
Content-Type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "c7d2a121-a121-c7d2-21a1-d2c721a1d2c7",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "9956b57f-b57f-9956-7fb5-56997fb55699",
  "skuPartNumber": "Sku Part Number value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "28bf4d7f-4d7f-28bf-7f4d-bf287f4dbf28",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "c7d2a121-a121-c7d2-21a1-d2c721a1d2c7",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "9956b57f-b57f-9956-7fb5-56997fb55699",
  "skuPartNumber": "Sku Part Number value"
}
```

