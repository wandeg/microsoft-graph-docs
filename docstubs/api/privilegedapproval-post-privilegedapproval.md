---
title: "Create privilegedApproval"
description: "Create a new privilegedApproval object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedApproval

Namespace: microsoft.graph

Create a new [privilegedApproval](../resources/privilegedapproval.md) object.

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
POST /privilegedApproval
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [privilegedApproval](../resources/privilegedapproval.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 441

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT1M41.0992332S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
  "endDateTime": "2016-12-31T23:57:26.2105705+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedapproval"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 490

{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "ca1728f7-28f7-ca17-f728-17caf72817ca",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "approvalType": "Approval Type value",
  "approvalState": "String",
  "approvalDuration": "-PT1M41.0992332S",
  "requestorReason": "Requestor Reason value",
  "approverReason": "Approver Reason value",
  "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
  "endDateTime": "2016-12-31T23:57:26.2105705+00:00"
}
```

