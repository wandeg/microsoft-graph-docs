---
title: "Update pendingSteps"
description: "Update the properties of a pendingSteps object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update pendingSteps

Namespace: microsoft.graph

Update the properties of a pendingSteps object.

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
PATCH /users/{usersId}/approvals/{approvalId}/pendingSteps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
  "name": "update_pendingsteps"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/approvals/{approvalId}/pendingSteps
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.approvalStep",
  "displayName": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
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
  "id": "e80cc81f-c81f-e80c-1fc8-0ce81fc80ce8",
  "displayName": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```

