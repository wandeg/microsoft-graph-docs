---
title: "Update deviceAppManagementTasks"
description: "Update the properties of a deviceAppManagementTasks object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceAppManagementTasks

Namespace: microsoft.graph

Update the properties of a deviceAppManagementTasks object.

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
PATCH /deviceAppManagement/deviceAppManagementTasks
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object.

The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/deviceappmanagementtask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|category|deviceAppManagementTaskCategory|**TODO: Add Description**. Possible values are: `unknown`, `advancedThreatProtection`.|
|priority|deviceAppManagementTaskPriority|**TODO: Add Description**. Possible values are: `none`, `high`, `low`.|
|creator|String|**TODO: Add Description**|
|creatorNotes|String|**TODO: Add Description**|
|assignedTo|String|**TODO: Add Description**|
|status|deviceAppManagementTaskStatus|**TODO: Add Description**. Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/deviceappmanagementtask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceappmanagementtasks"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-Type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "String",
  "description": "String",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
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
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "04c3a7a3-a7a3-04c3-a3a7-c304a3a7c304",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
}
```

