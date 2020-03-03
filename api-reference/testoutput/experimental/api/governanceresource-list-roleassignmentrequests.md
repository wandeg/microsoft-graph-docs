---
title: "List roleAssignmentRequests"
description: "Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roleAssignmentRequests

Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /governanceResources/{governanceResourcesId}/roleAssignmentRequests
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/governanceResources/{governanceResourcesId}/roleAssignmentRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governanceroleassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1197

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
      "id": "8b5623bd-23bd-8b56-bd23-568bbd23568b",
      "resourceId": "Resource Id value",
      "roleDefinitionId": "Role Definition Id value",
      "subjectId": "Subject Id value",
      "linkedEligibleRoleAssignmentId": "Linked Eligible Role Assignment Id value",
      "type": "Type value",
      "assignmentState": "Assignment State value",
      "requestedDateTime": "2016-12-31T23:59:36.6387568+03:00",
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
        "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
        "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
        "duration": "PT3M27.7161587S"
      }
    }
  ]
}
```

