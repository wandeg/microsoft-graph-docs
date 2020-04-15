---
title: "Add licenseDetails"
description: "Add licenseDetails by posting to the licenseDetails collection."
author: "**TODO: Provide Github Name**"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_licensedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/licenseDetails
Content-Type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "25ef5c03-5c03-25ef-035c-ef25035cef25",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "9f7a5a26-5a26-9f7a-265a-7a9f265a7a9f",
  "skuPartNumber": "Sku Part Number value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licensedetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "9c0a04cd-04cd-9c0a-cd04-0a9ccd040a9c",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "25ef5c03-5c03-25ef-035c-ef25035cef25",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "9f7a5a26-5a26-9f7a-265a-7a9f265a7a9f",
  "skuPartNumber": "Sku Part Number value"
}
```

