---
title: "Update completedSteps"
description: "Update the properties of a completedSteps object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update completedSteps

Namespace: microsoft.graph

Update the properties of a completedSteps object.

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
PATCH /invitations/{invitationsId}/invitedUser/approvals/{approvalId}/completedSteps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [approvalStep](../resources/approvalstep.md) object.

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
  "name": "update_completedsteps"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/approvals/{approvalId}/completedSteps
Content-Type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.approvalStep",
  "displayName": "Display Name value",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value"
  },
  "reviewedDateTime": "2017-01-01T00:02:48.7552683+00:00",
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
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

