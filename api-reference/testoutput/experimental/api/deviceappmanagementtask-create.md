---
title: "Create deviceAppManagementTask"
description: "Create a new deviceAppManagementTask object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceAppManagementTask

Namespace: microsoft.graph

Create a new [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/deviceappmanagementtask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name.|
|description|String|The description.|
|createdDateTime|DateTimeOffset|The created date.|
|dueDateTime|DateTimeOffset|The due date.|
|category|Enumeration|The category. Possible values are: `unknown`, `advancedThreatProtection`.|
|priority|Enumeration|The priority. Possible values are: `none`, `high`, `low`.|
|creator|String|The email address of the creator.|
|creatorNotes|String|Notes from the creator.|
|assignedTo|String|The name or email of the admin this task is assigned to.|
|status|Enumeration|The status. Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceappmanagementtask_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 383

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:01:36.4685818+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceappmanagementtask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 490

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "81fcc215-c215-81fc-15c2-fc8115c2fc81",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "dueDateTime": "2017-01-01T00:01:36.4685818+03:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

