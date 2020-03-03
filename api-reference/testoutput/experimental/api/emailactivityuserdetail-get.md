---
title: "Get emailActivityUserDetail"
description: "Read properties and relationships of the emailActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get emailActivityUserDetail

Read properties and relationships of the [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object.

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
GET ** Entity URI for microsoft.graph.emailActivityUserDetail not found
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
If successful, this method returns a `200 OK` response code and [emailActivityUserDetail](../resources/emailactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.emailActivityUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.emailActivityUserDetail",
    "id": "4ffc0b41-0b41-4ffc-410b-fc4f410bfc4f",
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
}
```

