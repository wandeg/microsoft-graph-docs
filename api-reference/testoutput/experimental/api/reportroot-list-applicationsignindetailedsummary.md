---
title: "List applicationSignInDetailedSummary"
description: "Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List applicationSignInDetailedSummary

Namespace: microsoft.graph

Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.

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
GET /reports/applicationSignInDetailedSummary
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/reports/applicationSignInDetailedSummary
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applicationsignindetailedsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applicationSignInDetailedSummary",
      "id": "2d7be85e-e85e-2d7b-5ee8-7b2d5ee87b2d",
      "appId": "App Id value",
      "appDisplayName": "App Display Name value",
      "status": {
        "@odata.type": "microsoft.graph.signInStatus",
        "errorCode": 9,
        "failureReason": "Failure Reason value",
        "additionalDetails": "Additional Details value"
      },
      "signInCount": 11,
      "aggregatedEventDateTime": "2017-01-01T00:01:04.3937333+03:00"
    }
  ]
}
```

