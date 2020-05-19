---
title: "Create pages"
description: "Create a new pages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create pages

Namespace: microsoft.graph

Create a new pages object.

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
POST /users/{usersId}/onenote/pages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onenotePage](../resources/onenotepage.md) object.

The following table shows the properties that are required when you create the [onenotePage](../resources/onenotepage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|title|String|**TODO: Add Description**|
|createdByAppId|String|**TODO: Add Description**|
|links|[pageLinks](../resources/pagelinks.md)|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|content|Stream|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|level|Int32|**TODO: Add Description**|
|order|Int32|**TODO: Add Description**|
|userTags|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [onenotePage](../resources/onenotepage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onenotepage_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/onenote/pages
Content-Type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.onenotePage",
  "self": "String",
  "title": "String",
  "createdByAppId": "String",
  "links": {
    "@odata.type": "microsoft.graph.pageLinks"
  },
  "contentUrl": "String",
  "content": "Stream",
  "level": "Integer",
  "order": "Integer",
  "userTags": [
    "String"
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotepage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onenotePage",
  "id": "728bc287-c287-728b-87c2-8b7287c28b72",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "title": "String",
  "createdByAppId": "String",
  "links": {
    "@odata.type": "microsoft.graph.pageLinks"
  },
  "contentUrl": "String",
  "content": "Stream",
  "lastModifiedDateTime": "String (timestamp)",
  "level": "Integer",
  "order": "Integer",
  "userTags": [
    "String"
  ]
}
```

