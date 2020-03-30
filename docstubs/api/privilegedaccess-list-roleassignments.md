---
title: "List roleAssignments"
description: "Get the governanceRoleAssignments from the roleAssignments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roleAssignments

Namespace: microsoft.graph

Get the governanceRoleAssignments from the roleAssignments navigation property.

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
GET /privilegedAccess/{privilegedAccessId}/roleAssignments
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/roleAssignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governanceroleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 667

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governanceRoleAssignment",
      "id": "fc86caf6-caf6-fc86-f6ca-86fcf6ca86fc",
      "resourceId": "Resource Id value",
      "roleDefinitionId": "Role Definition Id value",
      "subjectId": "Subject Id value",
      "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
      "externalId": "External Id value",
      "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
      "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
      "memberType": "Member Type value",
      "assignmentState": "Assignment State value",
      "status": "Status value"
    }
  ]
}
```

