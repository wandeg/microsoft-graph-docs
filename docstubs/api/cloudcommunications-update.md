---
title: "Update cloudCommunications"
description: "Update the properties of a cloudCommunications object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update cloudCommunications

Namespace: microsoft.graph

Update the properties of a [cloudCommunications](../resources/cloudcommunications.md) object.

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
PATCH /communications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [cloudCommunications](../resources/cloudcommunications.md) object.

The following table shows the properties that are required when you create the [cloudCommunications](../resources/cloudcommunications.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [cloudCommunications](../resources/cloudcommunications.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_cloudcommunications"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications
Content-type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.cloudCommunications"
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
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.cloudCommunications",
  "id": "053d1155-1155-053d-5511-3d0555113d05"
}
```

