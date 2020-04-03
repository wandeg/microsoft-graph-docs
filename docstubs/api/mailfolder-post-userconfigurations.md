---
title: "Add userConfigurations"
description: "Add userConfigurations by posting to the userConfigurations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userConfigurations

Namespace: microsoft.graph

Add userConfigurations by posting to the userConfigurations collection.

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
POST /me/mailFolders/{mailFolderId}/userConfigurations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [userConfiguration](../resources/userconfiguration.md) object.

The following table shows the properties that are required when you create the [userConfiguration](../resources/userconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|binaryData|Binary||



## Response
If successful, this method returns a `201 Created` response code and a [userConfiguration](../resources/userconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/mailFolders/{mailFolderId}/userConfigurations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.userconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 145

{
  "@odata.type": "#microsoft.graph.userConfiguration",
  "id": "80553fd8-3fd8-8055-d83f-5580d83f5580",
  "binaryData": "YmluYXJ5RGF0YQ=="
}
```

