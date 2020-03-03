---
title: "Create all"
description: "Create all by posting to the all collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create all

Create all by posting to the all collection.

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
POST /me/planner/all/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the plannerDelta object.

The following table shows the properties that are required when you create the plannerDelta.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [plannerDelta](../resources/plannerdelta.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannerdelta_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/planner/all
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.plannerDelta"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerdelta"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.plannerDelta",
  "id": "241acbc6-cbc6-241a-c6cb-1a24c6cb1a24"
}
```

