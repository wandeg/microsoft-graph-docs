---
title: "Update accessPackage"
description: "Update the properties of a accessPackage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackage

Namespace: microsoft.graph

Update the properties of a [accessPackage](../resources/accesspackage.md) object.

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
PATCH /accessPackages/{accessPackagesId}
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackage
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages/{accessPackageId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackage
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackage](../resources/accesspackage.md) object.

The following table shows the properties that are required when you create the [accessPackage](../resources/accesspackage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|catalogId|String||
|displayName|String||
|description|String||
|isHidden|Boolean||
|isRoleScopesVisible|Boolean||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.accessPackage",
  "catalogId": "Catalog Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isHidden": true,
  "isRoleScopesVisible": true,
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "7c78bc59-bc59-7c78-59bc-787c59bc787c",
  "catalogId": "Catalog Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isHidden": true,
  "isRoleScopesVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:01:10.7827862+00:00"
}
```

