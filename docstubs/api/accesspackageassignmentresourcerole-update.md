---
title: "Update accessPackageAssignmentResourceRole"
description: "Update the properties of a accessPackageAssignmentResourceRole object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageAssignmentResourceRole

Namespace: microsoft.graph

Update the properties of a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

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
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|originId|String||
|originSystem|String||
|status|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentresourcerole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}
Content-type: application/json
Content-length: 182

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
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
Content-Length: 231

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "id": "5791d32b-d32b-5791-2bd3-91572bd39157",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
}
```

