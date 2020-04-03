---
title: "updateRequest"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# updateRequest

Namespace: microsoft.graph



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
POST /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/updateRequest
POST /privilegedAccess/{privilegedAccessId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/updateRequest
POST /governanceResources/{governanceResourcesId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/updateRequest
POST /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/updateRequest
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|decision|String||
|assignmentState|String||
|schedule|[governanceSchedule](../resources/governanceschedule.md)||
|reason|String||



## Response
If successful, this action returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_updaterequest"
}
-->
``` http
POST https://graph.microsoft.com/beta/governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/updateRequest

Content-type: application/json
Content-length: 193

{
  "decision": "Decision value",
  "assignmentState": "Assignment State value",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule"
  },
  "reason": "Reason value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroleassignmentrequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 719

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
    "id": "0300e14c-e14c-0300-4ce1-00034ce10003",
    "resourceId": "Resource Id value",
    "roleDefinitionId": "Role Definition Id value",
    "subjectId": "Subject Id value",
    "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
    "type": "Type value",
    "assignmentState": "Assignment State value",
    "requestedDateTime": "2017-01-01T00:00:43.1895182+00:00",
    "reason": "Reason value",
    "status": {
      "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
    },
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule"
    }
  }
}
```

