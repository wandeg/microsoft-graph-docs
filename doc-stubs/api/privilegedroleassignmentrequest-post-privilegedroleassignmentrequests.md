---
title: "Create privilegedRoleAssignmentRequest"
description: "Create a new privilegedRoleAssignmentRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedRoleAssignmentRequest
Namespace: microsoft.graph

Create a new [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

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
POST /privilegedRoleAssignmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

The following table shows the properties that are required when you create the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|requestedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|duration|String|**TODO: Add Description**|
|reason|String|**TODO: Add Description**|
|ticketNumber|String|**TODO: Add Description**|
|ticketSystem|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignmentrequest_from_privilegedroleassignmentrequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-Type: application/json
Content-length: 427

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule"
  },
  "userId": "String",
  "roleId": "String",
  "type": "String",
  "assignmentState": "String",
  "requestedDateTime": "String (timestamp)",
  "status": "String",
  "duration": "String",
  "reason": "String",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "id": "e51ac914-c914-e51a-14c9-1ae514c91ae5",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule"
  },
  "userId": "String",
  "roleId": "String",
  "type": "String",
  "assignmentState": "String",
  "requestedDateTime": "String (timestamp)",
  "status": "String",
  "duration": "String",
  "reason": "String",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

