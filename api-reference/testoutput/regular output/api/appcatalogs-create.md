---
title: "Create appCatalogs"
description: "Create a new appCatalogs object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create appCatalogs

Namespace: microsoft.graph

Create a new [appCatalogs](../resources/appcatalogs.md) object.

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
POST ** Collection URI for microsoft.graph.appCatalogs not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [appCatalogs](../resources/appcatalogs.md) object.

The following table shows the properties that are required when you create the [appCatalogs](../resources/appcatalogs.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [appCatalogs](../resources/appcatalogs.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_appcatalogs_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.appCatalogs not found
Content-type: application/json
Content-length: 53

{
  "@odata.type": "#microsoft.graph.appCatalogs"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appcatalogs"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 102

{
  "@odata.type": "#microsoft.graph.appCatalogs",
  "id": "9ddb8195-8195-9ddb-9581-db9d9581db9d"
}
```

