---
title: "List userCredentialUsageDetailses"
description: "List properties and relationships of the userCredentialUsageDetails objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userCredentialUsageDetailses

List properties and relationships of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects.

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
GET /reports/userCredentialUsageDetails
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/reports/userCredentialUsageDetails
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
      "id": "4c03f248-f248-4c03-48f2-034c48f2034c",
      "feature": "String",
      "userPrincipalName": "User Principal Name value",
      "userDisplayName": "User Display Name value",
      "isSuccess": true,
      "authMethod": "String",
      "failureReason": "Failure Reason value",
      "eventDateTime": "2017-01-01T00:00:02.9716266+03:00"
    }
  ]
}
```

