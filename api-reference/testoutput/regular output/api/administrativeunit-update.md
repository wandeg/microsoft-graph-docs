---
title: "Update administrativeUnit"
description: "Update the properties of a administrativeUnit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update administrativeUnit

Namespace: microsoft.graph

Update the properties of a [administrativeUnit](../resources/administrativeunit.md) object.

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
PATCH ** Entity URI for microsoft.graph.administrativeUnit not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [administrativeUnit](../resources/administrativeunit.md) object.

The following table shows the properties that are required when you create the [administrativeUnit](../resources/administrativeunit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.administrativeUnit not found
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00"
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
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "e9ca2e59-2e59-e9ca-592e-cae9592ecae9",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00"
}
```

