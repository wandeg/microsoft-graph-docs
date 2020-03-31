---
title: "Update namedLocation"
description: "Update the properties of a namedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update namedLocation

Namespace: microsoft.graph

Update the properties of a [namedLocation](../resources/namedlocation.md) object.

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
PATCH /identity/conditionalAccess/namedLocations/{namedLocationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [namedLocation](../resources/namedlocation.md) object.

The following table shows the properties that are required when you create the [namedLocation](../resources/namedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [namedLocation](../resources/namedlocation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_namedlocation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/{namedLocationId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.namedLocation",
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
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.namedLocation",
  "id": "ad4bfca6-fca6-ad4b-a6fc-4bada6fc4bad",
  "displayName": "Display Name value",
  "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
  "modifiedDateTime": "2017-01-01T00:02:04.5847267+03:00"
}
```

