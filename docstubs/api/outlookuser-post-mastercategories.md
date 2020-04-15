---
title: "Add masterCategories"
description: "Add masterCategories by posting to the masterCategories collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add masterCategories

Namespace: microsoft.graph

Add masterCategories by posting to the masterCategories collection.

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
POST /me/outlook/masterCategories/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [outlookCategory](../resources/outlookcategory.md) object.

The following table shows the properties that are required when you create the [outlookCategory](../resources/outlookcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|color|categoryColor|**TODO: Add Description**. Possible values are: `preset0`, `preset1`, `preset2`, `preset3`, `preset4`, `preset5`, `preset6`, `preset7`, `preset8`, `preset9`, `preset10`, `preset11`, `preset12`, `preset13`, `preset14`, `preset15`, `preset16`, `preset17`, `preset18`, `preset19`, `preset20`, `preset21`, `preset22`, `preset23`, `preset24`, `none`.|



## Response
If successful, this method returns a `201 Created` response code and an [outlookCategory](../resources/outlookcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "displayName": "Display Name value",
  "color": "String"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookcategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "id": "6e5cd6e4-d6e4-6e5c-e4d6-5c6ee4d65c6e",
  "displayName": "Display Name value",
  "color": "String"
}
```

