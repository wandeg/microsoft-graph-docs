---
title: "Create governanceRoleAssignment"
description: "Create a new governanceRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create governanceRoleAssignment

Namespace: microsoft.graph

Create a new [governanceRoleAssignment](../resources/governanceroleassignment.md) object.

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
POST /governanceRoleAssignments
POST /privilegedAccess/{privilegedAccessId}/roleAssignments
POST /governanceResources/{governanceResourcesId}/roleAssignments
POST /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_governanceroleassignment_from_governanceroleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleAssignments
Content-type: application/json
Content-length: 537

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
  "status": "Status value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 586

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "id": "2f3eb365-b365-2f3e-65b3-3e2f65b33e2f",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
  "status": "Status value"
}
```

