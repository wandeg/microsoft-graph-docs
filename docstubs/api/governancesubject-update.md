---
title: "Update governanceSubject"
description: "Update the properties of a governanceSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update governanceSubject

Namespace: microsoft.graph

Update the properties of a [governanceSubject](../resources/governancesubject.md) object.

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
PATCH /governanceSubjects/{governanceSubjectsId}
PATCH /governanceRoleAssignments/{governanceRoleAssignmentsId}/subject
PATCH /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/subject
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/subject
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/subject
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [governanceSubject](../resources/governancesubject.md) object.

The following table shows the properties that are required when you create the [governanceSubject](../resources/governancesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|displayName|String||
|principalName|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceSubject](../resources/governancesubject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_governancesubject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/governanceSubjects/{governanceSubjectsId}
Content-type: application/json
Content-length: 195

{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
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
Content-Length: 244

{
  "@odata.type": "#microsoft.graph.governanceSubject",
  "id": "2b476e00-6e00-2b47-006e-472b006e472b",
  "type": "Type value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value"
}
```

