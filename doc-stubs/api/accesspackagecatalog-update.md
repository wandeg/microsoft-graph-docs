---
title: "Update accessPackageCatalog"
description: "Update the properties of an accessPackageCatalog object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageCatalog

Namespace: microsoft.graph

Update the properties of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

The following table shows the properties that are required when you create the [accessPackageCatalog](../resources/accesspackagecatalog.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|catalogType|String|**TODO: Add Description**|
|catalogStatus|String|**TODO: Add Description**|
|isExternallyVisible|Boolean|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}
Content-Type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "catalogStatus": "String",
  "isExternallyVisible": "Boolean",
  "createdBy": "String",
  "modifiedBy": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "ddf9ceca-ceca-ddf9-cace-f9ddcacef9dd",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "catalogStatus": "String",
  "isExternallyVisible": "Boolean",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

