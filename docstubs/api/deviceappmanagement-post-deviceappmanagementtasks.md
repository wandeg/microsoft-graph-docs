---
title: "Add deviceAppManagementTasks"
description: "Add deviceAppManagementTasks by posting to the deviceAppManagementTasks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceAppManagementTasks

Namespace: microsoft.graph

Add deviceAppManagementTasks by posting to the deviceAppManagementTasks collection.

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
POST /deviceAppManagement/deviceAppManagementTasks/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/deviceappmanagementtask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|createdDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|category|Enumeration| Possible values are: `unknown`, `advancedThreatProtection`.|
|priority|Enumeration| Possible values are: `none`, `high`, `low`.|
|creator|String||
|creatorNotes|String||
|assignedTo|String||
|status|Enumeration| Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceappmanagementtask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 383

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:01:30.9257409+00:00",
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
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "82127435-7435-8212-3574-128235741282",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
  "dueDateTime": "2017-01-01T00:01:30.9257409+00:00",
  "category": "String",
  "priority": "String",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "String"
}
```

