---
title: "Create administrativeUnit"
description: "Create a new administrativeUnit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create administrativeUnit

Namespace: microsoft.graph

Create a new [administrativeUnit](../resources/administrativeunit.md) object.

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
POST /administrativeUnits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}
-->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "e9ff2eb1-2eb1-e9ff-b12e-ffe9b12effe9",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

