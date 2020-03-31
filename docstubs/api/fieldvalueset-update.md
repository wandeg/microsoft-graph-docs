---
title: "Update fieldValueSet"
description: "Update the properties of a fieldValueSet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update fieldValueSet

Namespace: microsoft.graph

Update the properties of a [fieldValueSet](../resources/fieldvalueset.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/fields
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/versions/{listItemVersionId}/fields
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [fieldValueSet](../resources/fieldvalueset.md) object.

The following table shows the properties that are required when you create the [fieldValueSet](../resources/fieldvalueset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [fieldValueSet](../resources/fieldvalueset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_fieldvalueset"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/listItem/fields
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.fieldValueSet"
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
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.fieldValueSet",
  "id": "52069a1a-9a1a-5206-1a9a-06521a9a0652"
}
```

