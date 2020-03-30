---
title: "Add services"
description: "Add services by posting to the services collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add services

Namespace: microsoft.graph

Add services by posting to the services collection.

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
POST /print/services/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printService](../resources/printservice.md) object.

The following table shows the properties that are required when you create the [printService](../resources/printservice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [printService](../resources/printservice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printservice_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/services
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.printService"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printservice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.printService",
  "id": "c42ebf40-bf40-c42e-40bf-2ec440bf2ec4"
}
```

