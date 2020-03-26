---
title: "Create allowedDataLocation"
description: "Create a new allowedDataLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create allowedDataLocation

Namespace: microsoft.graph

Create a new [allowedDataLocation](../resources/alloweddatalocation.md) object.

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
POST /allowedDataLocations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [allowedDataLocation](../resources/alloweddatalocation.md) object.

The following table shows the properties that are required when you create the [allowedDataLocation](../resources/alloweddatalocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appId|String||
|location|String||
|isDefault|Boolean||
|domain|String||



## Response
If successful, this method returns a `201 Created` response code and a [allowedDataLocation](../resources/alloweddatalocation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_alloweddatalocation_from_alloweddatalocations"
}
-->
``` http
POST https://graph.microsoft.com/beta/allowedDataLocations
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.allowedDataLocation",
  "appId": "App Id value",
  "location": "Location value",
  "isDefault": true,
  "domain": "Domain value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alloweddatalocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.allowedDataLocation",
  "id": "e7473ab5-3ab5-e747-b53a-47e7b53a47e7",
  "appId": "App Id value",
  "location": "Location value",
  "isDefault": true,
  "domain": "Domain value"
}
```

