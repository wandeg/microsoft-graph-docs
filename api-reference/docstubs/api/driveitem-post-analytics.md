---
title: "Add analytics"
description: "Add analytics by posting to the analytics collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add analytics

Namespace: microsoft.graph

Add analytics by posting to the analytics collection.

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
POST /workbooks/{workbooksId}/analytics/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [itemAnalytics](../resources/itemanalytics.md) object.

The following table shows the properties that are required when you create the [itemAnalytics](../resources/itemanalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `204 No Content` response code and an [itemAnalytics](../resources/itemanalytics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_itemanalytics_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/analytics/$ref
Content-Type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.itemAnalytics"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemanalytics"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.itemAnalytics",
  "id": "ab310898-0898-ab31-9808-31ab980831ab"
}
```

