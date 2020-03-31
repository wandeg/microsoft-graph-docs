---
title: "Update programControlType"
description: "Update the properties of a programControlType object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update programControlType

Namespace: microsoft.graph

Update the properties of a [programControlType](../resources/programcontroltype.md) object.

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
PATCH /programControlTypes/{programControlTypesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [programControlType](../resources/programcontroltype.md) object.

The following table shows the properties that are required when you create the [programControlType](../resources/programcontroltype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|controlTypeGroupId|String||
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [programControlType](../resources/programcontroltype.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_programcontroltype"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/programControlTypes/{programControlTypesId}
Content-type: application/json
Content-length: 156

{
  "@odata.type": "#microsoft.graph.programControlType",
  "controlTypeGroupId": "Control Type Group Id value",
  "displayName": "Display Name value"
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
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.programControlType",
  "id": "e4f3b310-b310-e4f3-10b3-f3e410b3f3e4",
  "controlTypeGroupId": "Control Type Group Id value",
  "displayName": "Display Name value"
}
```

