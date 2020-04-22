---
title: "Get approvalStep"
description: "Read properties and relationships of an approvalStep object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get approvalStep

Namespace: microsoft.graph

Read properties and relationships of an [approvalStep](../resources/approvalstep.md) object.

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
GET /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps/{approvalStepId}
GET /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/completedSteps/{approvalStepId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps/{approvalStepId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "fce3def9-def9-fce3-f9de-e3fcf9dee3fc",
    "displayName": "Display Name value",
    "reviewedBy": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "reviewedDateTime": "2017-01-01T00:02:48.7552683+00:00",
    "reviewResult": "Review Result value",
    "justification": "Justification value"
  }
}
```

