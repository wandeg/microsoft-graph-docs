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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{privilegedApprovalId}
Content-type: application/json
Content-length: 440

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT3M6.6753994S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "aa3576a9-76a9-aa35-a976-35aaa97635aa",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT3M6.6753994S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00"
}
```

