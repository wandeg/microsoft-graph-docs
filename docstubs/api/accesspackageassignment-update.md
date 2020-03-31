---
title: "Update accessPackageAssignment"
description: "Update the properties of a accessPackageAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageAssignment

Namespace: microsoft.graph

Update the properties of a [accessPackageAssignment](../resources/accesspackageassignment.md) object.

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
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}
PATCH /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}/accessPackageAssignment
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageAssignments/{accessPackageAssignmentId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}/accessPackageAssignment
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageAssignments/{accessPackageAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignment](../resources/accesspackageassignment.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignment](../resources/accesspackageassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|catalogId|String||
|accessPackageId|String||
|assignmentPolicyId|String||
|targetId|String||
|assignmentStatus|String||
|assignmentState|String||
|isExtended|Boolean||
|expiredDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignment](../resources/accesspackageassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}
Content-type: application/json
Content-length: 419

{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "catalogId": "Catalog Id value",
  "accessPackageId": "Access Package Id value",
  "assignmentPolicyId": "Assignment Policy Id value",
  "targetId": "Target Id value",
  "assignmentStatus": "Assignment Status value",
  "assignmentState": "Assignment State value",
  "isExtended": true,
  "expiredDateTime": "2016-12-31T23:58:10.2887028+03:00"
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
Content-Length: 468

{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "1b52fa71-fa71-1b52-71fa-521b71fa521b",
  "catalogId": "Catalog Id value",
  "accessPackageId": "Access Package Id value",
  "assignmentPolicyId": "Assignment Policy Id value",
  "targetId": "Target Id value",
  "assignmentStatus": "Assignment Status value",
  "assignmentState": "Assignment State value",
  "isExtended": true,
  "expiredDateTime": "2016-12-31T23:58:10.2887028+03:00"
}
```

