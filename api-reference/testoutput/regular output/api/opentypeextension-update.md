---
title: "Update openTypeExtension"
description: "Update the properties of a openTypeExtension object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update openTypeExtension

Namespace: microsoft.graph

Update the properties of a [openTypeExtension](../resources/opentypeextension.md) object.

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
PATCH ** Entity URI for microsoft.graph.openTypeExtension not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [openTypeExtension](../resources/opentypeextension.md) object.

The following table shows the properties that are required when you create the [openTypeExtension](../resources/opentypeextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|extensionName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [openTypeExtension](../resources/opentypeextension.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.openTypeExtension not found
Content-type: application/json
Content-length: 103

{
  "@odata.type": "#microsoft.graph.openTypeExtension",
  "extensionName": "Extension Name value"
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
Content-Length: 152

{
  "@odata.type": "#microsoft.graph.openTypeExtension",
  "id": "02c7db78-db78-02c7-78db-c70278dbc702",
  "extensionName": "Extension Name value"
}
```

