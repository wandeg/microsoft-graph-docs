---
title: "Update governanceRoleAssignment"
description: "Update the properties of a governanceRoleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update governanceRoleAssignment

Namespace: microsoft.graph

Update the properties of a [governanceRoleAssignment](../resources/governanceroleassignment.md) object.

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
PATCH /governanceRoleAssignments/{governanceRoleAssignmentsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `200 OK` response code and an updated [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_governanceroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleAssignments/{governanceRoleAssignmentsId}
Content-Type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "assignmentState": "String",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governanceRoleAssignment",
  "id": "bd76e5a7-e5a7-bd76-a7e5-76bda7e576bd",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "assignmentState": "String",
  "status": "String"
}
```

