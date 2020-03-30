---
title: "Update outlookTaskGroup"
description: "Update the properties of a outlookTaskGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update outlookTaskGroup

Namespace: microsoft.graph

Update the properties of a [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/outlook/taskGroups/{outlookTaskGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

The following table shows the properties that are required when you create the [outlookTaskGroup](../resources/outlooktaskgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|changeKey|String||
|isDefaultGroup|Boolean||
|name|String||
|groupKey|Guid||



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/outlook/taskGroups/{outlookTaskGroupId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "40d990d5-90d5-40d9-d590-d940d590d940"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "id": "924488b9-88b9-9244-b988-4492b9884492",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "40d990d5-90d5-40d9-d590-d940d590d940"
}
```

