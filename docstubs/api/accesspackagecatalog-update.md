---
title: "Update accessPackageCatalog"
description: "Update the properties of a accessPackageCatalog object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageCatalog

Namespace: microsoft.graph

Update the properties of a [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

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
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
PATCH /accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}/accessPackageCatalog
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}/accessPackageCatalog
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

The following table shows the properties that are required when you create the [accessPackageCatalog](../resources/accesspackagecatalog.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|catalogType|String||
|catalogStatus|String||
|isExternallyVisible|Boolean||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "displayName": "Display Name value",
  "description": "Description value",
  "catalogType": "Catalog Type value",
  "catalogStatus": "Catalog Status value",
  "isExternallyVisible": true,
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
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
Content-Length: 499

{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "cf474770-4770-cf47-7047-47cf704747cf",
  "displayName": "Display Name value",
  "description": "Description value",
  "catalogType": "Catalog Type value",
  "catalogStatus": "Catalog Status value",
  "isExternallyVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:03:28.4967331+03:00"
}
```

