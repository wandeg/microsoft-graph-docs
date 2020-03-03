---
title: "Update windowsUniversalAppXContainedApp"
description: "Update the properties of a windowsUniversalAppXContainedApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsUniversalAppXContainedApp

Update the properties of a [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) object.

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
PATCH ** Entity URI for microsoft.graph.windowsUniversalAppXContainedApp not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/windowsUniversalAppXContainedApp.md) object.

The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appUserModelId|String|The app user model ID of the contained app of a WindowsUniversalAppX app.|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/windowsuniversalappxcontainedapp.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsuniversalappxcontainedapp"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.windowsUniversalAppXContainedApp not found
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
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
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "da92a4ce-a4ce-da92-cea4-92dacea492da",
  "appUserModelId": "App User Model Id value"
}
```

