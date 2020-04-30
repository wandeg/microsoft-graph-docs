---
title: "Update privilegedApproval"
description: "Update the properties of a privilegedApproval object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedApproval

Namespace: microsoft.graph

Update the properties of a [privilegedApproval](../resources/privilegedapproval.md) object.

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
PATCH /privilegedApproval/{privilegedApprovalId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
If successful, this method returns a `200 OK` response code and an updated [privilegedApproval](../resources/privilegedapproval.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{privilegedApprovalId}
Content-Type: application/json
Content-length: 354

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "userId": "String",
  "roleId": "String",
  "approvalType": "String",
  "approvalState": "String",
  "approvalDuration": "String (duration)",
  "requestorReason": "String",
  "approverReason": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "4e0d42c8-42c8-4e0d-c842-0d4ec8420d4e",
  "userId": "String",
  "roleId": "String",
  "approvalType": "String",
  "approvalState": "String",
  "approvalDuration": "String (duration)",
  "requestorReason": "String",
  "approverReason": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

