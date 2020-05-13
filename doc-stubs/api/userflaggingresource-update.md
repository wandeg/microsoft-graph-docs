---
title: "Update userFlaggingResource"
description: "Update the properties of a userFlaggingResource object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userFlaggingResource

Namespace: microsoft.graph

Update the properties of a [userFlaggingResource](../resources/userflaggingresource.md) object.

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
PATCH /userFlagging
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userFlaggingResource](../resources/userflaggingresource.md) object.

The following table shows the properties that are required when you create the [userFlaggingResource](../resources/userflaggingresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [userFlaggingResource](../resources/userflaggingresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userflaggingresource"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/userFlagging
Content-Type: application/json
Content-length: 62

{
  "@odata.type": "#microsoft.graph.userFlaggingResource"
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
  "@odata.type": "#microsoft.graph.userFlaggingResource",
  "id": "c353fd44-fd44-c353-44fd-53c344fd53c3"
}
```

