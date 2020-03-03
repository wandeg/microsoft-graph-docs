---
title: "Delete request"
description: "Deletes a request."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete request

Deletes a [request](../resources/request.md).

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
DELETE /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}
DELETE /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requestsAwaitingMyDecision/{requestId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_request"
}
-->
``` http
DELETE https://graph.microsoft.com/docs\api/approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

