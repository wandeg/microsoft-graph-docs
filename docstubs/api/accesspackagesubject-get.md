---
title: "Get accessPackageSubject"
description: "Read properties and relationships of the accessPackageSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageSubject

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.

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
GET /accessPackageAssignments/{accessPackageAssignmentsId}/target
GET /accessPackageResourceRequests/{accessPackageResourceRequestsId}/requestor
GET /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}/requestor
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageSubject
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/target
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests/{accessPackageResourceRequestId}/requestor
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}/requestor
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageSubject
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesubject"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/target
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageSubject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageSubject",
    "id": "736df86a-f86a-736d-6af8-6d736af86d73",
    "objectId": "Object Id value",
    "altSecId": "Alt Sec Id value",
    "displayName": "Display Name value",
    "principalName": "Principal Name value",
    "email": "Email value",
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "type": "Type value"
  }
}
```

