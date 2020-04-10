---
title: "List accessPackageAssignments"
description: "Get the accessPackageAssignments from the accessPackageAssignments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageAssignments

Namespace: microsoft.graph

Get the accessPackageAssignments from the accessPackageAssignments navigation property.

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
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageAssignments
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRoleId}/accessPackageAssignments
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageAssignments
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "685833c6-33c6-6858-c633-5868c6335868",
      "catalogId": "Catalog Id value",
      "accessPackageId": "Access Package Id value",
      "assignmentPolicyId": "Assignment Policy Id value",
      "targetId": "Target Id value",
      "assignmentStatus": "Assignment Status value",
      "assignmentState": "Assignment State value",
      "isExtended": true,
      "expiredDateTime": "2017-01-01T00:02:08.2864219+00:00"
    }
  ]
}
```

