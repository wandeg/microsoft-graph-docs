---
title: "Create macManagedAppProtection"
description: "Create a new macManagedAppProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create macManagedAppProtection

Namespace: microsoft.graph

Create a new [macManagedAppProtection](../resources/macmanagedappprotection.md) object.

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
POST ** Collection URI for microsoft.graph.macManagedAppProtection not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [macManagedAppProtection](../resources/macmanagedappprotection.md) object.

The following table shows the properties that are required when you create the [macManagedAppProtection](../resources/macmanagedappprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [macManagedAppProtection](../resources/macmanagedappprotection.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_macmanagedappprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.macManagedAppProtection not found
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.macmanagedappprotection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection",
  "id": "bac05fed-5fed-bac0-ed5f-c0baed5fc0ba"
}
```

