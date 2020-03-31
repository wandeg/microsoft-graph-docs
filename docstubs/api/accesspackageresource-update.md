---
title: "Update accessPackageResource"
description: "Update the properties of a accessPackageResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageResource

Namespace: microsoft.graph

Update the properties of a [accessPackageResource](../resources/accesspackageresource.md) object.

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
PATCH /accessPackageResources/{accessPackageResourcesId}
PATCH /identityGovernance/entitlementManagement/accessPackageResources/{accessPackageResourceId}
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources/{accessPackageResourceId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceScopes/{accessPackageResourceScopeId}/accessPackageResource
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageResource](../resources/accesspackageresource.md) object.

The following table shows the properties that are required when you create the [accessPackageResource](../resources/accesspackageresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|url|String||
|resourceType|String||
|originId|String||
|originSystem|String||
|isPendingOnboarding|Boolean||
|addedBy|String||
|addedOn|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageResource](../resources/accesspackageresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageResources/{accessPackageResourcesId}
Content-type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "displayName": "Display Name value",
  "description": "Description value",
  "url": "Url value",
  "resourceType": "Resource Type value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "isPendingOnboarding": true,
  "addedBy": "Added By value",
  "addedOn": "2016-12-31T23:57:56.6124592+03:00"
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
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "fa3fefe2-efe2-fa3f-e2ef-3ffae2ef3ffa",
  "displayName": "Display Name value",
  "description": "Description value",
  "url": "Url value",
  "resourceType": "Resource Type value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "isPendingOnboarding": true,
  "addedBy": "Added By value",
  "addedOn": "2016-12-31T23:57:56.6124592+03:00"
}
```

