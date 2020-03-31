---
title: "List licenseDetails"
description: "Get the licenseDetailses from the licenseDetails navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List licenseDetails

Namespace: microsoft.graph

Get the licenseDetailses from the licenseDetails navigation property.

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
GET /me/licenseDetails
GET /users/{usersId}/licenseDetails
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/licenseDetails
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.licensedetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 599

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.licenseDetails",
      "id": "6301dd2d-dd2d-6301-2ddd-01632ddd0163",
      "servicePlans": [
        {
          "@odata.type": "microsoft.graph.servicePlanInfo",
          "servicePlanId": "976809b7-09b7-9768-b709-6897b7096897",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "96e0d8ff-d8ff-96e0-ffd8-e096ffd8e096",
      "skuPartNumber": "Sku Part Number value"
    }
  ]
}
```

