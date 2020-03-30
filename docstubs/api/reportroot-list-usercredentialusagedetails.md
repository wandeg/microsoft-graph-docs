---
title: "List userCredentialUsageDetails"
description: "Get the userCredentialUsageDetailses from the userCredentialUsageDetails navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userCredentialUsageDetails

Namespace: microsoft.graph

Get the userCredentialUsageDetailses from the userCredentialUsageDetails navigation property.

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
GET /reports/userCredentialUsageDetails
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
If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.usercredentialusagedetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
      "id": "fdf4b730-b730-fdf4-30b7-f4fd30b7f4fd",
      "feature": "String",
      "userPrincipalName": "User Principal Name value",
      "userDisplayName": "User Display Name value",
      "isSuccess": true,
      "authMethod": "String",
      "failureReason": "Failure Reason value",
      "eventDateTime": "2017-01-01T00:02:22.1549518+03:00"
    }
  ]
}
```

