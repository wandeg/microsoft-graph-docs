---
title: "Update printerShare"
description: "Update the properties of a printerShare object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update printerShare

Namespace: microsoft.graph

Update the properties of a [printerShare](../resources/printershare.md) object.

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
PATCH /print/printerShares/{printerShareId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.

The following table shows the properties that are required when you create the [printerShare](../resources/printershare.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printerShares/{printerShareId}
Content-Type: application/json
Content-length: 79

{
  "@odata.type": "#microsoft.graph.printerShare",
  "name": "Name value"
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
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "8227d9b3-d9b3-8227-b3d9-2782b3d92782",
  "name": "Name value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
}
```

