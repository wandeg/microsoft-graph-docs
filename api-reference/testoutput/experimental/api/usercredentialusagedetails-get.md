---
title: "Get userCredentialUsageDetails"
description: "Read properties and relationships of the userCredentialUsageDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userCredentialUsageDetails

Namespace: microsoft.graph

Read properties and relationships of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

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
GET /reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}
-->
``` http
GET https://graph.microsoft.com/localtest/reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 430

{
  "value": {
    "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
    "id": "149bdb35-db35-149b-35db-9b1435db9b14",
    "feature": "String",
    "userPrincipalName": "User Principal Name value",
    "userDisplayName": "User Display Name value",
    "isSuccess": true,
    "authMethod": "String",
    "failureReason": "Failure Reason value",
    "eventDateTime": "2017-01-01T00:01:42.7768776+03:00"
  }
}
```

