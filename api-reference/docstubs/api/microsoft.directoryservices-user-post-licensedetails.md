---
title: "Create licenseDetails"
description: "Create a new licenseDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create licenseDetails

Namespace: Microsoft.DirectoryServices

Create a new licenseDetails object.

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
POST /me/licenseDetails
POST /users/{usersId}/licenseDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [licenseDetails](../resources/microsoft.directoryservices-licensedetails.md) object.

The following table shows the properties that are required when you create the [licenseDetails](../resources/microsoft.directoryservices-licensedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|servicePlans|[servicePlanInfo](../resources/microsoft.directoryservices-serviceplaninfo.md) collection|**TODO: Add Description**|
|skuId|Guid|**TODO: Add Description**|
|skuPartNumber|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [licenseDetails](../resources/microsoft.directoryservices-licensedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_licensedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/changelog/me/licenseDetails
Content-Type: application/json
Content-length: 489

{
  "@odata.type": "#Microsoft.DirectoryServices.licenseDetails",
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo",
      "servicePlanId": "4545cb79-cb79-4545-79cb-454579cb4545",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "92ad2f35-2f35-92ad-352f-ad92352fad92",
  "skuPartNumber": "Sku Part Number value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.licensedetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.licenseDetails",
  "id": "db8181df-81df-db81-df81-81dbdf8181db",
  "servicePlans": [
    {
      "@odata.type": "Microsoft.DirectoryServices.servicePlanInfo",
      "servicePlanId": "4545cb79-cb79-4545-79cb-454579cb4545",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "92ad2f35-2f35-92ad-352f-ad92352fad92",
  "skuPartNumber": "Sku Part Number value"
}
```

