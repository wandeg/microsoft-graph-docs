---
title: "Update deletedItems"
description: "Update the properties of a deletedItems object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deletedItems

Namespace: microsoft.graph

Update the properties of a deletedItems object.

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
PATCH /directory/deletedItems
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deleteditems"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/deletedItems
Content-Type: application/json
Content-length: 116

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00"
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
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "52a0dd76-dd76-52a0-76dd-a05276dda052",
  "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00"
}
```

