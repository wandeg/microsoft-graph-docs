---
title: "List accessPackageAssignmentRequests"
description: "List properties and relationships of the accessPackageAssignmentRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageAssignmentRequests

Namespace: microsoft.graph

List properties and relationships of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.

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
GET /accessPackageAssignmentRequests
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageAssignmentRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
      "id": "bf55d753-d753-bf55-53d7-55bf53d755bf",
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "isValidationOnly": true,
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "completedDate": "2016-12-31T23:57:08.7151202+03:00",
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "justification": "Justification value"
    }
  ]
}
```

