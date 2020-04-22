---
title: "businessFlow: recordDecisions"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# recordDecisions

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}/recordDecisions
POST /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision/{businessFlowId}/recordDecisions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|reviewResult|String|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "businessflow_recorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}/recordDecisions

Content-Type: application/json
Content-length: 88

{
  "reviewResult": "Review Result value",
  "justification": "Justification value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

