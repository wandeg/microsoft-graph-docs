---
title: "Create planner"
description: "Create a new planner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create planner

Namespace: microsoft.graph

Create a new [planner](../resources/planner.md) object.

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
POST ** Collection URI for microsoft.graph.planner not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [planner](../resources/planner.md) object.

The following table shows the properties that are required when you create the [planner](../resources/planner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [planner](../resources/planner.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_planner_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.planner not found
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.planner"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.planner",
  "id": "64ed2f2e-2f2e-64ed-2e2f-ed642e2fed64"
}
```

