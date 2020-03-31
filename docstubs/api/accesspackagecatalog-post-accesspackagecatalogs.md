---
title: "Create accessPackageCatalog"
description: "Create a new accessPackageCatalog object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageCatalog

Namespace: microsoft.graph

Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

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
POST /accessPackageCatalogs
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageCatalogs
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
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackagecatalog"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 498

{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "9b6f3ae7-3ae7-9b6f-e73a-6f9be73a6f9b",
  "displayName": "Display Name value",
  "description": "Description value",
  "catalogType": "Catalog Type value",
  "catalogStatus": "Catalog Status value",
  "isExternallyVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:01:43.3164239+03:00"
}
```

