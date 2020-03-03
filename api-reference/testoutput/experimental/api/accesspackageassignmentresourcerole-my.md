---
title: "My"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# My

Namespace: microsoft.graph



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
GET /accessPackageAssignmentResourceRoles/My
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/My
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentResourceRoles/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/My
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentresourcerole_my"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageAssignmentResourceRoles/My
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentresourcerole)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
      "id": "b14d540e-540e-b14d-0e54-4db10e544db1",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "status": "Status value"
    }
  ]
}
```

