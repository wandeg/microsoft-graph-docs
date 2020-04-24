---
title: "Update roleAssignmentRequests"
description: "Update the properties of a roleAssignmentRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update roleAssignmentRequests

Namespace: microsoft.graph

Update the properties of a roleAssignmentRequests object.

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
PATCH /governanceResources/{governanceResourcesId}/roleAssignmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.

The following table shows the properties that are required when you create the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|subjectId|String|**TODO: Add Description**|
|linkedEligibleRoleAssignmentId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|requestedDateTime|DateTimeOffset|**TODO: Add Description**|
|reason|String|**TODO: Add Description**|
|status|[governanceRoleAssignmentRequestStatus](../resources/governanceroleassignmentrequeststatus.md)|**TODO: Add Description**|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_roleassignmentrequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceResources/{governanceResourcesId}/roleAssignmentRequests
Content-Type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:01:27.8869422+03:00",
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
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "duration": "-PT0.9940994S"
  }
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
  "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
  "id": "c73e529c-529c-c73e-9c52-3ec79c523ec7",
  "resourceId": "Resource Id value",
  "roleDefinitionId": "Role Definition Id value",
  "subjectId": "Subject Id value",
  "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:01:27.8869422+03:00",
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
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "duration": "-PT0.9940994S"
  }
}
```

