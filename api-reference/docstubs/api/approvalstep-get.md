---
title: "Get approvalStep"
description: "Read the properties and relationships of an approvalStep object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get approvalStep

Namespace: microsoft.graph

Read the properties and relationships of an [approvalStep](../resources/approvalstep.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/approvals/{approvalId}/pendingSteps/{approvalStepId}
GET /me/approvals/{approvalId}/completedSteps/{approvalStepId}
GET /users/{usersId}/approvals/{approvalId}/pendingSteps/{approvalStepId}
GET /users/{usersId}/approvals/{approvalId}/completedSteps/{approvalStepId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [approvalStep](../resources/approvalstep.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_approvalstep"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/approvals/{approvalId}/pendingSteps/{approvalStepId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.approvalStep",
    "id": "e80cc81f-c81f-e80c-1fc8-0ce81fc80ce8",
    "displayName": "String",
    "reviewedBy": {
      "@odata.type": "microsoft.graph.identity"
    },
    "reviewedDateTime": "String (timestamp)",
    "reviewResult": "String",
    "justification": "String"
  }
}
```

