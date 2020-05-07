---
title: "List deviceAppManagementTasks"
description: "Get the deviceAppManagementTasks from the deviceAppManagementTasks navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceAppManagementTasks

Namespace: microsoft.graph

Get the deviceAppManagementTasks from the deviceAppManagementTasks navigation property.

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
GET /deviceAppManagement/deviceAppManagementTasks
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/deviceappmanagementtask.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_deviceappmanagementtask"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceappmanagementtask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

