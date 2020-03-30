---
title: "Create accessPackage"
description: "Create a new accessPackage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackage

Namespace: microsoft.graph

Create a new [accessPackage](../resources/accesspackage.md) object.

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
POST /accessPackages
POST /identityGovernance/entitlementManagement/accessPackages
POST /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackages
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "00a1dc82-dc82-00a1-82dc-a10082dca100",
  "catalogId": "Catalog Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isHidden": true,
  "isRoleScopesVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:00:40.3078262+00:00"
}
```

