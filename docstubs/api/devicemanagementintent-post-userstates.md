---
title: "Add userStates"
description: "Add userStates by posting to the userStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userStates

Namespace: microsoft.graph

Add userStates by posting to the userStates collection.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||
|userName|String||
|deviceCount|Int32||
|lastReportedDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementintentuserstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2016-12-31T23:57:45.8617849+00:00",
  "state": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintentuserstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "b15fa0a4-a0a4-b15f-a4a0-5fb1a4a05fb1",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2016-12-31T23:57:45.8617849+00:00",
  "state": "String"
}
```

