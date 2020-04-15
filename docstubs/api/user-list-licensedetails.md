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
  ]
}
```

