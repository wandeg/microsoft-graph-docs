---
title: "Add settings"
description: "Add settings by posting to the settings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add settings

Namespace: microsoft.graph

Add settings by posting to the settings collection.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|definitionId|String||
|valueJson|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementsettinginstance_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
Content-type: application/json
Content-length: 151

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementsettinginstance"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 200

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "da3bef94-ef94-da3b-94ef-3bda94ef3bda",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

