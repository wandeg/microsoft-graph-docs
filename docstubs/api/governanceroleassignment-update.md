---
title: "Update governanceRoleAssignment"
description: "Update the properties of a governanceRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update governanceRoleAssignment

Namespace: microsoft.graph

Update the properties of a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.

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
PATCH /governanceRoleAssignments/{governanceRoleAssignmentsId}
PATCH /privilegedAccess/{privilegedAccessId}/roleAssignments/{governanceRoleAssignmentId}
PATCH /governanceResources/{governanceResourcesId}/roleAssignments/{governanceRoleAssignmentId}
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [governanceRoleAssignment](../resources/governanceroleassignment.md) object.

The following table shows the properties that are required when you create the [governanceRoleAssignment](../resources/governanceroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|roleDefinitionId|String||
|subjectId|String||
|linkedEligibleRoleAssignmentId|String||
|externalId|String||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|memberType|String||
|assignmentState|String||
|status|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_governanceroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleAssignments/{governanceRoleAssignmentsId}
Content-type: application/json
Content-length: 537

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
  "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
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
Content-Length: 586

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "id": "50174b32-4b32-5017-324b-1750324b1750",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
  "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
  "status": "Status value"
}
```

