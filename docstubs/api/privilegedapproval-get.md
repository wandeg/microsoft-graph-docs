---
title: "Get privilegedApproval"
description: "Read properties and relationships of the privilegedApproval object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get privilegedApproval

Namespace: microsoft.graph

Read properties and relationships of the [privilegedApproval](../resources/privilegedapproval.md) object.

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
GET /privilegedApproval/{privilegedApprovalId}
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
If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval/{privilegedApprovalId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedApproval",
    "id": "9b1eb282-b282-9b1e-82b2-1e9b82b21e9b",
    "userId": "User Id value",
    "roleId": "Role Id value",
    "approvalType": "Approval Type value",
    "approvalState": "String",
    "approvalDuration": "PT34.4337974S",
    "requestorReason": "Requestor Reason value",
    "approverReason": "Approver Reason value",
    "startDateTime": "2016-12-31T23:57:40.5444496+00:00",
    "endDateTime": "2016-12-31T23:58:47.51829+00:00"
  }
}
```

