---
title: "accessPackageAssignment: My"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# My

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /accessPackageAssignments/My
GET /identityGovernance/entitlementManagement/accessPackageAssignments/My
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageAssignments/My
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [accessPackageAssignment](../resources/accesspackageassignment.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignments/My
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignment",
      "id": "6f11a7e3-a7e3-6f11-e3a7-116fe3a7116f",
      "catalogId": "Catalog Id value",
      "accessPackageId": "Access Package Id value",
      "assignmentPolicyId": "Assignment Policy Id value",
      "targetId": "Target Id value",
      "assignmentStatus": "Assignment Status value",
      "assignmentState": "Assignment State value",
      "isExtended": true,
      "expiredDateTime": "2016-12-31T23:57:03.8636442+03:00"
    }
  ]
}
```

