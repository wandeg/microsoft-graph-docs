---
title: "Add intents"
description: "Add intents by posting to the intents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add intents

Namespace: microsoft.graph

Add intents by posting to the intents collection.

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
POST /deviceManagement/intents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/devicemanagementintent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementintent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "8611e186-e186-8611-86e1-118686e11186",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

