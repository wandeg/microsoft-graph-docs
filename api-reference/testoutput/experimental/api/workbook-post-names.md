---
title: "Add names"
description: "Add names by posting to the names collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add names

Add names by posting to the names collection.

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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the workbookNamedItem object.

The following table shows the properties that are required when you create the workbookNamedItem.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|comment|String||
|name|String||
|scope|String||
|type|String||
|value|[Json](../resources/Json.md)||
|visible|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooknameditem_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooknameditem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "id": "8e64bc7c-bc7c-8e64-7cbc-648e7cbc648e",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
}
```

