---
title: "Get accessPackageAssignmentPolicy"
description: "Read properties and relationships of the accessPackageAssignmentPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageAssignmentPolicy

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

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
GET /accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentPolicy
GET /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentPolicy
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 653

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
    "id": "3c72b1ab-b1ab-3c72-abb1-723cabb1723c",
    "userType": "User Type value",
    "accessPackageId": "Access Package Id value",
    "displayName": "Display Name value",
    "description": "Description value",
    "isEnabled": true,
    "canExtend": true,
    "durationInDays": 14,
    "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
    "createdBy": "Created By value",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "modifiedBy": "Modified By value",
    "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00"
  }
}
```

