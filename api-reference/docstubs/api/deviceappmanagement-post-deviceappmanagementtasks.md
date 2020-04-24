---
title: "Create deviceAppManagementTasks"
description: "Create a new deviceAppManagementTasks object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceAppManagementTasks

Namespace: microsoft.graph

Create a new deviceAppManagementTasks object.

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
POST /deviceAppManagement/deviceAppManagementTasks
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/deviceappmanagementtask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The name.|
|description|String|The description.|
|createdDateTime|DateTimeOffset|The created date.|
|dueDateTime|DateTimeOffset|The due date.|
|category|deviceAppManagementTaskCategory|The category. Possible values are: `unknown`, `advancedThreatProtection`.|
|priority|deviceAppManagementTaskPriority|The priority. Possible values are: `none`, `high`, `low`.|
|creator|String|The email address of the creator.|
|creatorNotes|String|Notes from the creator.|
|assignedTo|String|The name or email of the admin this task is assigned to.|
|status|deviceAppManagementTaskStatus|The status. Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceappmanagementtask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-Type: application/json
Content-length: 383

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:03:16.4480136+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceappmanagementtask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "1e08dcac-dcac-1e08-acdc-081eacdc081e",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "dueDateTime": "2017-01-01T00:03:16.4480136+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

