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
|Header|Value|
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
GET https://graph.microsoft.com/localtest/me/licenseDetails
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
      "id": "c98f110d-110d-c98f-0d11-8fc90d118fc9",
      "servicePlans": [
        {
          "@odata.type": "microsoft.graph.servicePlanInfo",
          "servicePlanId": "430099a8-99a8-4300-a899-0043a8990043",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "25470e04-0e04-2547-040e-4725040e4725",
      "skuPartNumber": "Sku Part Number value"
    }
  ]
}
```

