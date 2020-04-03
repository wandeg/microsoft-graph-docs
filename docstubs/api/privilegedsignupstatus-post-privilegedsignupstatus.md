---
title: "Create privilegedSignupStatus"
description: "Create a new privilegedSignupStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedSignupStatus

Namespace: microsoft.graph

Create a new [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

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
POST /privilegedSignupStatus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

The following table shows the properties that are required when you create the [privilegedSignupStatus](../resources/privilegedsignupstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isRegistered|Boolean||
|status|Enumeration| Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|



## Response
If successful, this method returns a `201 Created` response code and a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedsignupstatus_from_privilegedsignupstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedSignupStatus
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "isRegistered": true,
  "status": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedsignupstatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "id": "7086705f-705f-7086-5f70-86705f708670",
  "isRegistered": true,
  "status": "String"
}
```

