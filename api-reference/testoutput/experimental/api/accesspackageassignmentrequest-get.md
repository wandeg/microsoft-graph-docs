---
title: "Get accessPackageAssignmentRequest"
description: "Read properties and relationships of the accessPackageAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageAssignmentRequest

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.

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
GET /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
    "id": "732f916a-916a-732f-6a91-2f736a912f73",
    "requestType": "Request Type value",
    "requestState": "Request State value",
    "requestStatus": "Request Status value",
    "isValidationOnly": true,
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "completedDate": "2016-12-31T23:58:45.2006324+03:00",
    "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
    "justification": "Justification value"
  }
}
```

