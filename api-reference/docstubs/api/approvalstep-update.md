---
title: "Update approvalStep"
description: "Update the properties of an approvalStep object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update approvalStep

Namespace: microsoft.graph

Update the properties of an [approvalStep](../resources/approvalstep.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps/{approvalStepId}
PATCH /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/completedSteps/{approvalStepId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [approvalStep](../resources/approvalstep.md) object.

The following table shows the properties that are required when you create the [approvalStep](../resources/approvalstep.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|reviewedBy|[identity](../resources/identity.md)|**TODO: Add Description**|
|reviewedDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewResult|String|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [approvalStep](../resources/approvalstep.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_approvalstep"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/approvals/{approvalId}/pendingSteps/{approvalStepId}
Content-Type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.approvalStep",
  "displayName": "Display Name value",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value"
  },
  "reviewedDateTime": "2016-12-31T23:58:44.4686785+03:00",
  "reviewResult": "Review Result value",
  "justification": "Justification value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

