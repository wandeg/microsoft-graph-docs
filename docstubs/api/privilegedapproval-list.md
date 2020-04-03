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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedApproval
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedapproval)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedApproval",
      "id": "ca1728f7-28f7-ca17-f728-17caf72817ca",
      "userId": "User Id value",
      "roleId": "Role Id value",
      "approvalType": "Approval Type value",
      "approvalState": "String",
      "approvalDuration": "-PT1M41.0992332S",
      "requestorReason": "Requestor Reason value",
      "approverReason": "Approver Reason value",
      "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
      "endDateTime": "2016-12-31T23:57:26.2105705+00:00"
    }
  ]
}
```

