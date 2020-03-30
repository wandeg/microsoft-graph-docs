---
title: "Update conditionalAccessRoot"
description: "Update the properties of a conditionalAccessRoot object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update conditionalAccessRoot

Namespace: microsoft.graph

Update the properties of a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.

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
PATCH /conditionalAccess
PATCH /identity/conditionalAccess
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.

The following table shows the properties that are required when you create the [conditionalAccessRoot](../resources/conditionalaccessroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [conditionalAccessRoot](../resources/conditionalaccessroot.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccessroot"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/conditionalAccess
Content-type: application/json
Content-length: 63

{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot"
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
Content-Length: 112

{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot",
  "id": "dee2b881-b881-dee2-81b8-e2de81b8e2de"
}
```

