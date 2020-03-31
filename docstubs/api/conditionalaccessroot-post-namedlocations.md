---
title: "Add namedLocations"
description: "Add namedLocations by posting to the namedLocations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add namedLocations

Namespace: microsoft.graph

Add namedLocations by posting to the namedLocations collection.

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
POST /identity/conditionalAccess/namedLocations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [namedLocation](../resources/namedlocation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.namedlocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.namedLocation",
  "id": "bf66a940-a940-bf66-40a9-66bf40a966bf",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "modifiedDateTime": "2017-01-01T00:03:28.4967331+03:00"
}
```

