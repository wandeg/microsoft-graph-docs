---
title: "Update userConfiguration"
description: "Update the properties of a userConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userConfiguration

Namespace: microsoft.graph

Update the properties of a [userConfiguration](../resources/userconfiguration.md) object.

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
PATCH /me/mailFolders/{mailFolderId}/userConfigurations/{userConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userConfiguration](../resources/userconfiguration.md) object.

The following table shows the properties that are required when you create the [userConfiguration](../resources/userconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|binaryData|Binary||



## Response
If successful, this method returns a `200 OK` response code and an updated [userConfiguration](../resources/userconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/mailFolders/{mailFolderId}/userConfigurations/{userConfigurationId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.userConfiguration",
  "binaryData": "YmluYXJ5RGF0YQ=="
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
Content-Length: 145

{
  "@odata.type": "#microsoft.graph.userConfiguration",
  "id": "298b037d-037d-298b-7d03-8b297d038b29",
  "binaryData": "YmluYXJ5RGF0YQ=="
}
```

