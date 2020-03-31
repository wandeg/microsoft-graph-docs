---
title: "Update accessPackageSubject"
description: "Update the properties of a accessPackageSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageSubject

Namespace: microsoft.graph

Update the properties of a [accessPackageSubject](../resources/accesspackagesubject.md) object.

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
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/target
PATCH /accessPackageResourceRequests/{accessPackageResourceRequestsId}/requestor
PATCH /accessPackageAssignmentRequests/{accessPackageAssignmentRequestsId}/requestor
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageSubject
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/target
PATCH /identityGovernance/entitlementManagement/accessPackageResourceRequests/{accessPackageResourceRequestId}/requestor
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentRequests/{accessPackageAssignmentRequestId}/requestor
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageSubject
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageSubject](../resources/accesspackagesubject.md) object.

The following table shows the properties that are required when you create the [accessPackageSubject](../resources/accesspackagesubject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|objectId|String||
|altSecId|String||
|displayName|String||
|principalName|String||
|email|String||
|onPremisesSecurityIdentifier|String||
|type|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageSubject](../resources/accesspackagesubject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackagesubject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/target
Content-type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
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
Content-Length: 392

{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "2282e1e2-e1e2-2282-e2e1-8222e2e18222",
  "objectId": "Object Id value",
  "altSecId": "Alt Sec Id value",
  "displayName": "Display Name value",
  "principalName": "Principal Name value",
  "email": "Email value",
  "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
  "type": "Type value"
}
```

