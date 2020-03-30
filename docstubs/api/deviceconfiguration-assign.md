---
title: "assign"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# assign

Namespace: microsoft.graph



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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|deviceConfigurationGroupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection||
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "deviceconfiguration_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 613

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "588314db-14db-5883-db14-8358db148358",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d6456c9d-6c9d-d645-9d6c-45d69d6c45d6",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "String",
      "sourceId": "Source Id value"
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceconfigurationassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d6456c9d-6c9d-d645-9d6c-45d69d6c45d6",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "String",
      "sourceId": "Source Id value"
    }
  ]
}
```

