---
title: "Add acceptedSenders"
description: "Add acceptedSenders by posting to the acceptedSenders collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add acceptedSenders

Namespace: microsoft.graph

Add acceptedSenders by posting to the acceptedSenders collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /groups/{groupsId}/acceptedSenders/$ref
POST /me/joinedGroups/{groupId}/acceptedSenders/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [directoryObject](../resources/directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/acceptedSenders
Content-type: application/json
Content-length: 115

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "2017-01-01T00:00:54.363956+03:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 164

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "c7fd4a95-4a95-c7fd-954a-fdc7954afdc7",
  "deletedDateTime": "2017-01-01T00:00:54.363956+03:00"
}
```

