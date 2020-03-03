---
title: "Create value"
description: "Create value by posting to the value collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create value

Namespace: microsoft.graph

Create value by posting to the value collection.

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
POST ** Collection URI for microsoft.graph.deviceManagementSettingInstance not found/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|definitionId|String|The ID of the setting definition for this instance|
|valueJson|String|JSON representation of the value|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementsettinginstance_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceManagementSettingInstance not found
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
  "id": "0d6aa03a-a03a-0d6a-3aa0-6a0d3aa06a0d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

