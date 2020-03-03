---
title: "Create groupPolicyConfigurationAssignment"
description: "Create a new groupPolicyConfigurationAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupPolicyConfigurationAssignment

Namespace: microsoft.graph

Create a new [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.

The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The type of groups targeted the group policy configuration.|



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicyconfigurationassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicyconfigurationassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "b4a4b34d-b34d-b4a4-4db3-a4b44db3a4b4",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

