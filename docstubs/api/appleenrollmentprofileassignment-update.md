---
title: "Update appleEnrollmentProfileAssignment"
description: "Update the properties of a appleEnrollmentProfileAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update appleEnrollmentProfileAssignment

Namespace: microsoft.graph

Update the properties of a [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.

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
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.

The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_appleenrollmentprofileassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "cb181570-1570-cb18-7015-18cb701518cb",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

