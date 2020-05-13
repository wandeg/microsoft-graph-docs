---
title: "Create fill"
description: "Create a new fill object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create fill

Namespace: microsoft.graph

Create a new fill object.

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
POST /workbookRange/format/fill
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeFill](../resources/workbookrangefill.md) object.

The following table shows the properties that are required when you create the [workbookRangeFill](../resources/workbookrangefill.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|color|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookrangefill_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/workbookRange/format/fill
Content-Type: application/json
Content-length: 81

{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "color": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangefill"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "id": "7724273d-273d-7724-3d27-24773d272477",
  "color": "String"
}
```

