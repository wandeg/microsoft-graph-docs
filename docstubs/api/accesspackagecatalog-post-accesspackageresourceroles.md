---
title: "Add accessPackageResourceRoles"
description: "Add accessPackageResourceRoles by posting to the accessPackageResourceRoles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageResourceRoles

Namespace: microsoft.graph

Add accessPackageResourceRoles by posting to the accessPackageResourceRoles collection.

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
POST /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceRoles/$ref
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResourceRoles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|originId|String||
|originSystem|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerole_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceRoles
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 271

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "id": "3a4d30d0-30d0-3a4d-d030-4d3ad0304d3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value"
}
```

