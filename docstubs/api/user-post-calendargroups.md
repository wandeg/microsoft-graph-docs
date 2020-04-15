---
title: "Add calendarGroups"
description: "Add calendarGroups by posting to the calendarGroups collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add calendarGroups

Namespace: microsoft.graph

Add calendarGroups by posting to the calendarGroups collection.

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
POST /me/calendarGroups/$ref
POST /users/{usersId}/calendarGroups/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [calendarGroup](../resources/calendargroup.md) object.

The following table shows the properties that are required when you create the [calendarGroup](../resources/calendargroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|classId|Guid|**TODO: Add Description**|
|changeKey|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [calendarGroup](../resources/calendargroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "name": "Name value",
  "classId": "2dcabce0-bce0-2dca-e0bc-ca2de0bcca2d",
  "changeKey": "Change Key value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendargroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "fb125bdb-5bdb-fb12-db5b-12fbdb5b12fb",
  "name": "Name value",
  "classId": "2dcabce0-bce0-2dca-e0bc-ca2de0bcca2d",
  "changeKey": "Change Key value"
}
```

