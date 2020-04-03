---
title: "Create accessPackageAssignmentRequest"
description: "Create a new accessPackageAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageAssignmentRequest

Namespace: microsoft.graph

Create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.

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
POST /accessPackageAssignmentRequests
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
POST /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageAssignmentRequests
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "completedDate": "2017-01-01T00:01:54.8809963+00:00",
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "justification": "Justification value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "3ccc96a8-96a8-3ccc-a896-cc3ca896cc3c",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "completedDate": "2017-01-01T00:01:54.8809963+00:00",
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "justification": "Justification value"
}
```

