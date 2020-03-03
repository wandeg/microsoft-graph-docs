---
title: "Create workbookRangeBorder"
description: "Create a new workbookRangeBorder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookRangeBorder

Namespace: microsoft.graph

Create a new [workbookRangeBorder](../resources/workbookrangeborder.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.workbookRangeBorder not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookRangeBorder](../resources/workbookrangeborder.md) object.

The following table shows the properties that are required when you create the [workbookRangeBorder](../resources/workbookrangeborder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|color|String||
|sideIndex|String||
|style|String||
|weight|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookrangeborder_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeBorder not found
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "color": "Color value",
  "sideIndex": "Side Index value",
  "style": "Style value",
  "weight": "Weight value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangeborder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "id": "98eb73a4-73a4-98eb-a473-eb98a473eb98",
  "color": "Color value",
  "sideIndex": "Side Index value",
  "style": "Style value",
  "weight": "Weight value"
}
```

