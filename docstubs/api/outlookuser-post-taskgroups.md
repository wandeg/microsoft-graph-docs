---
title: "Add taskGroups"
description: "Add taskGroups by posting to the taskGroups collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add taskGroups

Namespace: microsoft.graph

Add taskGroups by posting to the taskGroups collection.

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
POST /me/outlook/taskGroups/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

The following table shows the properties that are required when you create the [outlookTaskGroup](../resources/outlooktaskgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|changeKey|String|**TODO: Add Description**|
|isDefaultGroup|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|groupKey|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-Type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "be26f387-f387-be26-87f3-26be87f326be"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlooktaskgroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "id": "a6049a9c-9a9c-a604-9c9a-04a69c9a04a6",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "be26f387-f387-be26-87f3-26be87f326be"
}
```

