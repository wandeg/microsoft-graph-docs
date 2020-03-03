---
title: "Create auditLogRoot"
description: "Create a new auditLogRoot object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create auditLogRoot

Namespace: microsoft.graph

Create a new [auditLogRoot](../resources/auditlogroot.md) object.

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
POST ** Collection URI for microsoft.graph.auditLogRoot not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [auditLogRoot](../resources/auditlogroot.md) object.

The following table shows the properties that are required when you create the [auditLogRoot](../resources/auditlogroot.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [auditLogRoot](../resources/auditlogroot.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_auditlogroot_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.auditLogRoot not found
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.auditLogRoot"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditlogroot"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.auditLogRoot",
  "id": "0e6fe61e-e61e-0e6f-1ee6-6f0e1ee66f0e"
}
```

