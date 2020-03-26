---
title: "Update privilegedSignupStatus"
description: "Update the properties of a privilegedSignupStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedSignupStatus

Namespace: microsoft.graph

Update the properties of a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

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
PATCH /privilegedSignupStatus/{privilegedSignupStatusId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

The following table shows the properties that are required when you create the [privilegedSignupStatus](../resources/privilegedsignupstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isRegistered|Boolean||
|status|Enumeration|. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedsignupstatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedSignupStatus/{privilegedSignupStatusId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "id": "e4508abd-8abd-e450-bd8a-50e4bd8a50e4",
  "isRegistered": true,
  "status": "String"
}
```

