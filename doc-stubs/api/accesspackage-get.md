---
title: "Get accessPackage"
description: "Read the properties and relationships of an accessPackage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get accessPackage

Namespace: microsoft.graph

Read the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.

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
GET /accessPackages/{accessPackagesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackage",
    "id": "8fbf40b4-40b4-8fbf-b440-bf8fb440bf8f",
    "catalogId": "String",
    "displayName": "String",
    "description": "String",
    "isHidden": "Boolean",
    "isRoleScopesVisible": "Boolean",
    "createdBy": "String",
    "createdDateTime": "String (timestamp)",
    "modifiedBy": "String",
    "modifiedDateTime": "String (timestamp)"
  }
}
```

