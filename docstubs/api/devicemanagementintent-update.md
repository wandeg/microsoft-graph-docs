---
title: "Update deviceManagementIntent"
description: "Update the properties of a deviceManagementIntent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementIntent

Namespace: microsoft.graph

Update the properties of a [deviceManagementIntent](../resources/devicemanagementintent.md) object.

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
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/devicemanagementintent.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/devicemanagementintent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|isAssigned|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|templateId|String||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/devicemanagementintent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementintent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
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
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "0d149074-9074-0d14-7490-140d7490140d",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

