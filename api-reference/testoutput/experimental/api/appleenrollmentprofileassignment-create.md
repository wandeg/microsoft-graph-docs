---
title: "Create appleEnrollmentProfileAssignment"
description: "Create a new appleEnrollmentProfileAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create appleEnrollmentProfileAssignment

Namespace: microsoft.graph

Create a new [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.

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
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.

The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The assignment target for the Apple user initiated deployment profile.|



## Response
If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_appleenrollmentprofileassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
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
  "@odata.type": "microsoft.graph.appleenrollmentprofileassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "c52ec797-c797-c52e-97c7-2ec597c72ec5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

