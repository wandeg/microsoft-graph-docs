---
title: "Update resources"
description: "Update the properties of a resources object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update resources

Namespace: microsoft.graph

Update the properties of a resources object.

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
PATCH /users/{usersId}/onenote/resources
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

If successful, this method returns a `200 OK` response code and an updated [onenoteResource](../resources/onenoteresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_resources"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/onenote/resources
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "0d518272-8272-0d51-7282-510d7282510d",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```

