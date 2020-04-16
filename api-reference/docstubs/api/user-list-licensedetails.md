---
title: "List licenseDetails"
description: "Get the licenseDetails from the licenseDetails navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List licenseDetails

Namespace: microsoft.graph

Get the licenseDetails from the licenseDetails navigation property.

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
GET /me/licenseDetails
GET /users/{usersId}/licenseDetails
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/licenseDetails
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.licensedetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.licenseDetails",
      "id": "e8f5bae1-bae1-e8f5-e1ba-f5e8e1baf5e8",
      "servicePlans": [
        {
          "@odata.type": "microsoft.graph.servicePlanInfo",
          "servicePlanId": "15efb390-b390-15ef-90b3-ef1590b3ef15",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "220e6177-6177-220e-7761-0e2277610e22",
      "skuPartNumber": "Sku Part Number value"
    }
  ]
}
```

