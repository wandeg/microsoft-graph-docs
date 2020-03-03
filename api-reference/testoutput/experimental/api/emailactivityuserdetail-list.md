---
title: "List emailActivityUserDetails"
description: "List properties and relationships of the emailActivityUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List emailActivityUserDetails

Namespace: microsoft.graph

List properties and relationships of the [emailActivityUserDetail](../resources/emailactivityuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.emailActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [emailActivityUserDetail](../resources/emailactivityuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailActivityUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailactivityuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailActivityUserDetail",
      "id": "aa341e5f-1e5f-aa34-5f1e-34aa5f1e34aa",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "displayName": "Display Name value",
      "isDeleted": true,
      "deletedDate": "Date",
      "lastActivityDate": "Date",
      "sendCount": 9,
      "receiveCount": 12,
      "readCount": 9,
      "assignedProducts": [
        "Assigned Products value"
      ],
      "reportPeriod": "Report Period value"
    }
  ]
}
```

