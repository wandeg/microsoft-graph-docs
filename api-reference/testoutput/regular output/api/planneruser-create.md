---
title: "Create plannerUser"
description: "Create a new plannerUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create plannerUser

Namespace: microsoft.graph

Create a new [plannerUser](../resources/planneruser.md) object.

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
POST ** Collection URI for microsoft.graph.plannerUser not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [plannerUser](../resources/planneruser.md) object.

The following table shows the properties that are required when you create the [plannerUser](../resources/planneruser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [plannerUser](../resources/planneruser.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_planneruser_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.plannerUser not found
Content-type: application/json
Content-length: 53

{
  "@odata.type": "#microsoft.graph.plannerUser"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planneruser"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 102

{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "ff260b91-0b91-ff26-910b-26ff910b26ff"
}
```

