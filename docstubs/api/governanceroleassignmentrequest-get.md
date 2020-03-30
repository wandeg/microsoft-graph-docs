---
title: "Get governanceRoleAssignmentRequest"
description: "Read properties and relationships of the governanceRoleAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governanceRoleAssignmentRequest

Namespace: microsoft.graph

Read properties and relationships of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.

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
GET /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}
GET /privilegedAccess/{privilegedAccessId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
GET /governanceResources/{governanceResourcesId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
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
If successful, this method returns a `200 OK` response code and [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1127

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
    "id": "bd5ae2c2-e2c2-bd5a-c2e2-5abdc2e25abd",
    "resourceId": "Resource Id value",
    "roleDefinitionId": "Role Definition Id value",
    "subjectId": "Subject Id value",
    "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
    "type": "Type value",
    "assignmentState": "Assignment State value",
    "requestedDateTime": "2016-12-31T23:58:10.9963224+03:00",
    "reason": "Reason value",
    "status": {
      "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus",
      "status": "Status value",
      "subStatus": "Sub Status value",
      "statusDetails": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ]
    },
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule",
      "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
      "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
      "duration": "PT3M32.4915489S"
    }
  }
}
```

