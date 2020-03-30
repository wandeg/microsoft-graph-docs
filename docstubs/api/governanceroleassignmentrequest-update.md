---
title: "Update governanceRoleAssignmentRequest"
description: "Update the properties of a governanceRoleAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update governanceRoleAssignmentRequest

Namespace: microsoft.graph

Update the properties of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.

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
PATCH /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}
PATCH /privilegedAccess/{privilegedAccessId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
PATCH /governanceResources/{governanceResourcesId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.

The following table shows the properties that are required when you create the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceId|String||
|roleDefinitionId|String||
|subjectId|String||
|linkedEligibleRoleAssignmentId|String||
|type|String||
|assignmentState|String||
|requestedDateTime|DateTimeOffset||
|reason|String||
|status|[governanceRoleAssignmentRequestStatus](../resources/governanceroleassignmentrequeststatus.md)||
|schedule|[governanceSchedule](../resources/governanceschedule.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_governanceroleassignmentrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}
Content-type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2016-12-31T23:59:52.0455003+00:00",
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
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
    "duration": "PT10.2249944S"
  }
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
Content-Length: 1050

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "id": "f8a9f244-f244-f8a9-44f2-a9f844f2a9f8",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2016-12-31T23:59:52.0455003+00:00",
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
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
    "duration": "PT10.2249944S"
  }
}
```

