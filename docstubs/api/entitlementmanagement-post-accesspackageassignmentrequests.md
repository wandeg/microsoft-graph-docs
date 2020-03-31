---
title: "Add accessPackageAssignmentRequests"
description: "Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageAssignmentRequests

Namespace: microsoft.graph

Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/$ref
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
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "completedDate": "2016-12-31T23:57:56.9044756+03:00",
  "expirationDateTime": "2016-12-31T23:57:21.3858094+03:00",
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
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "102bf6a4-f6a4-102b-a4f6-2b10a4f62b10",
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "isValidationOnly": true,
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "completedDate": "2016-12-31T23:57:56.9044756+03:00",
  "expirationDateTime": "2016-12-31T23:57:21.3858094+03:00",
  "justification": "Justification value"
}
```

