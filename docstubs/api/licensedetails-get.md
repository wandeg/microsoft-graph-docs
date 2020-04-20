---
title: "Get licenseDetails"
description: "Read properties and relationships of a licenseDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get licenseDetails

Namespace: microsoft.graph

Read properties and relationships of a [licenseDetails](../resources/licensedetails.md) object.

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
GET /me/licenseDetails/{licenseDetailsId}
GET /users/{usersId}/licenseDetails/{licenseDetailsId}
GET /invitations/{invitationsId}/invitedUser/licenseDetails/{licenseDetailsId}
GET /servicePrincipals/{servicePrincipalsId}/licenseDetails/{licenseDetailsId}
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
If successful, this method returns a `200 OK` response code and a [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/licenseDetails/{licenseDetailsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

