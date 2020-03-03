---
title: "Create financials"
description: "Create a new financials object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create financials

Namespace: microsoft.graph

Create a new [financials](../resources/financials.md) object.

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
POST ** Collection URI for microsoft.graph.financials not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [financials](../resources/financials.md) object.

The following table shows the properties that are required when you create the [financials](../resources/financials.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [financials](../resources/financials.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_financials_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.financials not found
Content-type: application/json
Content-length: 52

{
  "@odata.type": "#microsoft.graph.financials"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.financials"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.financials",
  "id": "278b3623-3623-278b-2336-8b2723368b27"
}
```

