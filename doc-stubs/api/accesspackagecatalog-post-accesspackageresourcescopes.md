---
title: "Create accessPackageResourceScopes"
description: "Create a new accessPackageResourceScopes object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageResourceScopes

Namespace: microsoft.graph

Create a new accessPackageResourceScopes object.

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
POST /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceScope](../resources/accesspackageresourcescope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|
|roleOriginId|String|**TODO: Add Description**|
|isRootScope|Boolean|**TODO: Add Description**|
|url|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcescope_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResourceScopes
Content-Type: application/json
Content-length: 256

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "isRootScope": "Boolean",
  "url": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcescope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "id": "049c0de6-0de6-049c-e60d-9c04e60d9c04",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "isRootScope": "Boolean",
  "url": "String"
}
```

