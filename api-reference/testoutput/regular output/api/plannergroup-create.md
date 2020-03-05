---
title: "Create plannerGroup"
description: "Create a new plannerGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create plannerGroup

Namespace: microsoft.graph

Create a new [plannerGroup](../resources/plannergroup.md) object.

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
POST ** Collection URI for microsoft.graph.plannerGroup not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [plannerGroup](../resources/plannergroup.md) object.

The following table shows the properties that are required when you create the [plannerGroup](../resources/plannergroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [plannerGroup](../resources/plannergroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannergroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.plannerGroup not found
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.plannerGroup"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannergroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.plannerGroup",
  "id": "551c0bd7-0bd7-551c-d70b-1c55d70b1c55"
}
```

