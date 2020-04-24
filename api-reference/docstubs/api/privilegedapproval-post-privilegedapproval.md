---
title: "Create privilegedApproval"
description: "Create a new privilegedApproval object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedApproval

Namespace: microsoft.graph

Create a new [privilegedApproval](../resources/privilegedapproval.md) object.

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
POST /privilegedApproval
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [privilegedApproval](../resources/privilegedapproval.md) object.

The following table shows the properties that are required when you create the [privilegedApproval](../resources/privilegedapproval.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|approvalType|String|**TODO: Add Description**|
|approvalState|approvalState|**TODO: Add Description**. Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalDuration|Duration|**TODO: Add Description**|
|requestorReason|String|**TODO: Add Description**|
|approverReason|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [privilegedApproval](../resources/privilegedapproval.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-Type: application/json
Content-length: 441

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT1M43.8104246S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedapproval"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "fe571cdc-1cdc-fe57-dc1c-57fedc1c57fe",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT1M43.8104246S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00"
}
```

