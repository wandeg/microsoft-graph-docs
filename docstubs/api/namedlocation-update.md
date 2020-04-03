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
  "id": "047c157e-157e-047c-7e15-7c047e157c04",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00"
}
```

