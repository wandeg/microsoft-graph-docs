---
title: "Create microsoftStoreForBusinessContainedApp"
description: "Create a new microsoftStoreForBusinessContainedApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create microsoftStoreForBusinessContainedApp

Namespace: microsoft.graph

Create a new [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object.

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
POST ** Collection URI for microsoft.graph.microsoftStoreForBusinessContainedApp not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object.

The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appUserModelId|String|The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.|



## Response
If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/microsoftstoreforbusinesscontainedapp.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_microsoftstoreforbusinesscontainedapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.microsoftStoreForBusinessContainedApp not found
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftstoreforbusinesscontainedapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "e2cae680-e680-e2ca-80e6-cae280e6cae2",
  "appUserModelId": "App User Model Id value"
}
```

