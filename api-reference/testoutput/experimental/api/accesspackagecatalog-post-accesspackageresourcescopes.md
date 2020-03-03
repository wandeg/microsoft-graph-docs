---
title: "Add accessPackageResourceScopes"
description: "Add accessPackageResourceScopes by posting to the accessPackageResourceScopes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageResourceScopes

Add accessPackageResourceScopes by posting to the accessPackageResourceScopes collection.

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
POST /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes/$ref
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResourceScopes/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the accessPackageResourceScope object.

The following table shows the properties that are required when you create the accessPackageResourceScope.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|originId|String||
|originSystem|String||
|roleOriginId|String||
|isRootScope|Boolean||
|url|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcescope_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "roleOriginId": "Role Origin Id value",
  "isRootScope": true,
  "url": "Url value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcescope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 362

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "id": "f2526dba-6dba-f252-ba6d-52f2ba6d52f2",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "roleOriginId": "Role Origin Id value",
  "isRootScope": true,
  "url": "Url value"
}
```

