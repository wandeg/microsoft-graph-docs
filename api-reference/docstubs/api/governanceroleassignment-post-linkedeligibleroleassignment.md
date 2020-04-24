---
title: "Add linkedEligibleRoleAssignment"
description: "Add linkedEligibleRoleAssignment by posting to the linkedEligibleRoleAssignment collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add linkedEligibleRoleAssignment

Namespace: microsoft.graph

Add linkedEligibleRoleAssignment by posting to the linkedEligibleRoleAssignment collection.

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
POST /governanceRoleAssignments/{governanceRoleAssignmentsId}/linkedEligibleRoleAssignment/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [governanceRoleAssignment](../resources/governanceroleassignment.md) object.

The following table shows the properties that are required when you create the [governanceRoleAssignment](../resources/governanceroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|subjectId|String|**TODO: Add Description**|
|linkedEligibleRoleAssignmentId|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|memberType|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and a [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governanceroleassignment_from_governanceroleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleAssignments/{governanceRoleAssignmentsId}/linkedEligibleRoleAssignment/$ref
Content-Type: application/json
Content-length: 537

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
  "status": "Status value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroleassignment"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "id": "dae219cc-19cc-dae2-cc19-e2dacc19e2da",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "externalId": "External Id value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "memberType": "Member Type value",
  "assignmentState": "Assignment State value",
  "status": "Status value"
}
```

