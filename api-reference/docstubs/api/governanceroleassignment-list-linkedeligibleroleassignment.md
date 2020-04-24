---
title: "List linkedEligibleRoleAssignment"
description: "Get the governanceRoleAssignments from the linkedEligibleRoleAssignment navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List linkedEligibleRoleAssignment

Namespace: microsoft.graph

Get the governanceRoleAssignments from the linkedEligibleRoleAssignment navigation property.

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
GET /governanceRoleAssignments/{governanceRoleAssignmentsId}/linkedEligibleRoleAssignment
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceRoleAssignments/{governanceRoleAssignmentsId}/linkedEligibleRoleAssignment
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governanceroleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

