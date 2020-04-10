---
title: "List privilegedApprovals"
description: "List properties and relationships of the privilegedApproval objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedApprovals

Namespace: microsoft.graph

List properties and relationships of the [privilegedApproval](../resources/privilegedapproval.md) objects.

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
GET /privilegedApproval
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
If successful, this method returns a `200 OK` response code and a collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedapproval)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 564

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedApproval",
      "id": "978886a6-86a6-9788-a686-8897a6868897",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "approvalType": "Approval Type value",
      "approvalState": "String",
      "approvalDuration": "PT2M4.825446S",
      "requestorReason": "Requestor Reason value",
      "approverReason": "Approver Reason value",
      "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
      "endDateTime": "2017-01-01T00:02:08.1909286+00:00"
    }
  ]
}
```

