---
title: "List accessPackageAssignmentPolicies"
description: "List properties and relationships of the accessPackageAssignmentPolicy objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageAssignmentPolicies

Namespace: microsoft.graph

List properties and relationships of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.

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
GET /accessPackageAssignmentPolicies
GET /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackageAssignmentPolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 694

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
      "id": "76099350-9350-7609-5093-097650930976",
      "userType": "User Type value",
      "accessPackageId": "Access Package Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "isEnabled": true,
      "canExtend": true,
      "durationInDays": 14,
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00"
    }
  ]
}
```

