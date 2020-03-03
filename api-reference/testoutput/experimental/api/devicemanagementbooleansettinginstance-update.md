---
title: "Update deviceManagementBooleanSettingInstance"
description: "Update the properties of a deviceManagementBooleanSettingInstance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementBooleanSettingInstance

Namespace: microsoft.graph

Update the properties of a [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object.

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
PATCH ** Entity URI for microsoft.graph.deviceManagementBooleanSettingInstance not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object.

The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|
|value|Boolean|The boolean value|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementbooleansettinginstance"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.deviceManagementBooleanSettingInstance not found
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
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
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "6e381c2f-1c2f-6e38-2f1c-386e2f1c386e",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

