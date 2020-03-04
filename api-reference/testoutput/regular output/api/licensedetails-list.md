---
title: "List licenseDetailses"
description: "List properties and relationships of the licenseDetails objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List licenseDetailses

Namespace: microsoft.graph

List properties and relationships of the [licenseDetails](../resources/licensedetails.md) objects.

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
GET /me/licenseDetails
GET /users/{usersId}/licenseDetails
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.

## Example

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
      "id": "2fc67f94-7f94-2fc6-947f-c62f947fc62f",
      "servicePlans": [
        {
          "@odata.type": "microsoft.graph.servicePlanInfo",
          "servicePlanId": "52357315-7315-5235-1573-355215733552",
          "servicePlanName": "Service Plan Name value",
          "provisioningStatus": "Provisioning Status value",
          "appliesTo": "Applies To value"
        }
      ],
      "skuId": "ca7e2026-2026-ca7e-2620-7eca26207eca",
      "skuPartNumber": "Sku Part Number value"
    }
  ]
}
```

