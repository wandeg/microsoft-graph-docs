---
title: "Update accessPackageAssignmentRequest"
description: "Update the properties of a accessPackageAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageAssignmentRequest

Namespace: microsoft.graph

Update the properties of a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.

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
PATCH /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|requestType|String||
|requestState|String||
|requestStatus|String||
|isValidationOnly|Boolean||
|createdDateTime|DateTimeOffset||
|completedDate|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|justification|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "completedDate": "2017-01-01T00:00:26.0295417+03:00",
  "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
  "justification": "Justification value"
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
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "172da47d-a47d-172d-7da4-2d177da42d17",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "completedDate": "2017-01-01T00:00:26.0295417+03:00",
  "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
  "justification": "Justification value"
}
```

