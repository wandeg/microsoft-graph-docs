---
title: "Update assignments"
description: "Update the properties of an assignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update assignments

Namespace: microsoft.graph

Update the properties of an assignments object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the device health script assignment entity. This property is read-only.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The Azure Active Directory group we are targeting the script to|
|runRemediationScript|Boolean|Determine whether we want to run detection script only or run both detection script and remediation script|
|runSchedule|[runSchedule](../resources/runschedule.md)|Script run schedule for the target group|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_assignments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
Content-Type: application/json
Content-length: 336

{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptAssignment",
  "target": {
    "@odata.type": "microsoft.management.services.api.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": "Boolean",
  "runSchedule": {
    "@odata.type": "microsoft.management.services.api.runSchedule"
  }
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
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptAssignment",
  "id": "b8c0078d-078d-b8c0-8d07-c0b88d07c0b8",
  "target": {
    "@odata.type": "microsoft.management.services.api.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": "Boolean",
  "runSchedule": {
    "@odata.type": "microsoft.management.services.api.runSchedule"
  }
}
```

