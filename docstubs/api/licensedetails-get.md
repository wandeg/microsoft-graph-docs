---
title: "Get licenseDetails"
description: "Read properties and relationships of the licenseDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get licenseDetails

Namespace: microsoft.graph

Read properties and relationships of the [licenseDetails](../resources/licensedetails.md) object.

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
GET /me/licenseDetails/{licenseDetailsId}
GET /users/{usersId}/licenseDetails/{licenseDetailsId}
GET /servicePrincipals/{servicePrincipalsId}/licenseDetails/{licenseDetailsId}
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
If successful, this method returns a `200 OK` response code and [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/licenseDetails/{licenseDetailsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": {
    "@odata.type": "#microsoft.graph.licenseDetails",
    "id": "8be603c6-03c6-8be6-c603-e68bc603e68b",
    "servicePlans": [
      {
        "@odata.type": "microsoft.graph.servicePlanInfo",
        "servicePlanId": "835ae98c-e98c-835a-8ce9-5a838ce95a83",
        "servicePlanName": "Service Plan Name value",
        "provisioningStatus": "Provisioning Status value",
        "appliesTo": "Applies To value"
      }
    ],
    "skuId": "76ed7b76-7b76-76ed-767b-ed76767bed76",
    "skuPartNumber": "Sku Part Number value"
  }
}
```

