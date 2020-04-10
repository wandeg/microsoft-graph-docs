---
title: "Add roleAssignmentRequests"
description: "Add roleAssignmentRequests by posting to the roleAssignmentRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleAssignmentRequests

Namespace: microsoft.graph

Add roleAssignmentRequests by posting to the roleAssignmentRequests collection.

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
POST /privilegedAccess/{privilegedAccessId}/roleAssignmentRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governanceroleassignmentrequest_from_governanceroleassignmentrequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedAccess/{privilegedAccessId}/roleAssignmentRequests
Content-type: application/json
Content-length: 1004

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2016-12-31T23:57:01.4951864+00:00",
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
    "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
    "endDateTime": "2017-01-01T00:02:08.1909286+00:00",
    "duration": "-PT2M44.7705843S"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceroleassignmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "id": "20fee40c-e40c-20fe-0ce4-fe200ce4fe20",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2016-12-31T23:57:01.4951864+00:00",
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
    "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
    "endDateTime": "2017-01-01T00:02:08.1909286+00:00",
    "duration": "-PT2M44.7705843S"
  }
}
```

