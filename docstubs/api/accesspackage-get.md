---
title: "Get accessPackage"
description: "Read properties and relationships of the accessPackage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackage

Namespace: microsoft.graph

Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.

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
GET /accessPackages/{accessPackagesId}
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackage
GET /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages/{accessPackageId}
GET /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackage
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}
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
If successful, this method returns a `200 OK` response code and [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 506

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackage",
    "id": "99c2a26f-a26f-99c2-6fa2-c2996fa2c299",
    "catalogId": "Catalog Id value",
    "displayName": "Display Name value",
    "description": "Description value",
    "isHidden": true,
    "isRoleScopesVisible": true,
    "createdBy": "Created By value",
    "createdDateTime": "2016-12-31T23:59:31.6288943+00:00",
    "modifiedBy": "Modified By value",
    "modifiedDateTime": "2016-12-31T23:57:53.4522402+00:00"
  }
}
```

