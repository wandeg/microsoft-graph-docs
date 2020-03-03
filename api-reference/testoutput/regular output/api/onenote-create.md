---
title: "Create onenote"
description: "Create a new onenote object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create onenote

Namespace: microsoft.graph

Create a new [onenote](../resources/onenote.md) object.

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
POST ** Collection URI for microsoft.graph.onenote not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [onenote](../resources/onenote.md) object.

The following table shows the properties that are required when you create the [onenote](../resources/onenote.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [onenote](../resources/onenote.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onenote_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.onenote not found
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.onenote"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.onenote",
  "id": "fce0c053-c053-fce0-53c0-e0fc53c0e0fc"
}
```

