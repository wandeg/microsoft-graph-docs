---
title: "Create resources"
description: "Create a new resources object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create resources

Namespace: microsoft.graph

Create a new resources object.

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
POST /users/{usersId}/onenote/resources
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onenoteResource](../resources/onenoteresource.md) object.

The following table shows the properties that are required when you create the [onenoteResource](../resources/onenoteresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|content|Stream|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [onenoteResource](../resources/onenoteresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onenoteresource_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/onenote/resources
Content-Type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "3250fd3e-fd3e-3250-3efd-50323efd5032",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```

