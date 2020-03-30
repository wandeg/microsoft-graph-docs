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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /accessPackageAssignments/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/My
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageAssignments/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageAssignments/My
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageAssignment](../resources/accesspackageassignment.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignments/My
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignment",
      "id": "3eebfb6e-fb6e-3eeb-6efb-eb3e6efbeb3e",
      "catalogId": "Catalog Id value",
      "accessPackageId": "Access Package Id value",
      "assignmentPolicyId": "Assignment Policy Id value",
      "targetId": "Target Id value",
      "assignmentStatus": "Assignment Status value",
      "assignmentState": "Assignment State value",
      "isExtended": true,
      "expiredDateTime": "2016-12-31T23:56:39.2358551+00:00"
    }
  ]
}
```

