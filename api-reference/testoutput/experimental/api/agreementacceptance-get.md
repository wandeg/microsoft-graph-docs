---
title: "Get agreementAcceptance"
description: "Read properties and relationships of the agreementAcceptance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get agreementAcceptance

Read properties and relationships of the [agreementAcceptance](../resources/agreementacceptance.md) object.

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
GET /agreementAcceptances/{agreementAcceptancesId}
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
If successful, this method returns a `200 OK` response code and [agreementAcceptance](../resources/agreementacceptance.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/agreementAcceptances/{agreementAcceptancesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.agreementAcceptance",
    "id": "8e86a9a0-a9a0-8e86-a0a9-868ea0a9868e",
    "agreementId": "Agreement Id value",
    "userId": "User Id value",
    "agreementFileId": "Agreement File Id value",
    "recordedDateTime": "2017-01-01T00:03:18.9258587+03:00",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "userEmail": "User Email value",
    "state": "String"
  }
}
```

