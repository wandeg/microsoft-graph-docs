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
PATCH /administrativeUnits/{administrativeUnitsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [administrativeUnit](../resources/administrativeunit.md) object.

The following table shows the properties that are required when you create the [administrativeUnit](../resources/administrativeunit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String||
|description|String||
|visibility|String||



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
PATCH https://graph.microsoft.com/beta/administrativeUnits/{administrativeUnitsId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
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
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "2e2ecb61-cb61-2e2e-61cb-2e2e61cb2e2e",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

