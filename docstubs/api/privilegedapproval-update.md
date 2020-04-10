---
title: "Update privilegedApproval"
description: "Update the properties of a privilegedApproval object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedApproval

Namespace: microsoft.graph

Update the properties of a [privilegedApproval](../resources/privilegedapproval.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedApproval](../resources/privilegedapproval.md) object.

The following table shows the properties that are required when you create the [privilegedApproval](../resources/privilegedapproval.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userId|String||
|roleId|String||
|approvalType|String||
|approvalState|Enumeration| Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalDuration|Duration||
|requestorReason|String||
|approverReason|String||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||



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
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "PT2M4.825446S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "endDateTime": "2017-01-01T00:02:08.1909286+00:00"
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
Content-Length: 487

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "978886a6-86a6-9788-a686-8897a6868897",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "PT2M4.825446S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
  "endDateTime": "2017-01-01T00:02:08.1909286+00:00"
}
```

