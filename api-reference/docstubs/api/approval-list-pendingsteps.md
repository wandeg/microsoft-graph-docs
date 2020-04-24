---
title: "List pendingSteps"
description: "Get the approvalSteps from the pendingSteps navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List pendingSteps

Namespace: microsoft.graph

Get the approvalSteps from the pendingSteps navigation property.

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
GET /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps
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
If successful, this method returns a `200 OK` response code and a collection of [approvalStep](../resources/approvalstep.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_approvalstep"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approvalstep)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.approvalStep",
      "id": "3c86e66a-e66a-3c86-6ae6-863c6ae6863c",
      "displayName": "Display Name value",
      "reviewedBy": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "reviewedDateTime": "2016-12-31T23:58:44.4686785+03:00",
      "reviewResult": "Review Result value",
      "justification": "Justification value"
    }
  ]
}
```

