---
title: "Update accessPackages"
description: "Update the properties of an accessPackages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackages

Namespace: microsoft.graph

Update the properties of an accessPackages object.

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
PATCH /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackage](../resources/accesspackage.md) object.

The following table shows the properties that are required when you create the [accessPackage](../resources/accesspackage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|catalogId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|isHidden|Boolean|**TODO: Add Description**|
|isRoleScopesVisible|Boolean|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackages"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages
Content-Type: application/json
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
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "79d75bbb-5bbb-79d7-bb5b-d779bb5bd779",
  "catalogId": "Catalog Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isHidden": true,
  "isRoleScopesVisible": true,
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00"
}
```

