---
title: "Create profile"
description: "Create a new profile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create profile

Namespace: microsoft.graph

Create a new [profile](../resources/profile.md) object.

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
POST ** Collection URI for microsoft.graph.profile not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [profile](../resources/profile.md) object.

The following table shows the properties that are required when you create the [profile](../resources/profile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [profile](../resources/profile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_profile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.profile not found
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.profile"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.profile",
  "id": "e4dae4fb-e4fb-e4da-fbe4-dae4fbe4dae4"
}
```

