---
title: "Update tenantSetupInfo"
description: "Update the properties of a tenantSetupInfo object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update tenantSetupInfo

Namespace: microsoft.graph

Update the properties of a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.

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
PATCH ** Entity URI for microsoft.graph.tenantSetupInfo not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [tenantSetupInfo](../resources/tenantsetupinfo.md) object.

The following table shows the properties that are required when you create the [tenantSetupInfo](../resources/tenantsetupinfo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userRolesActions|String||
|firstTimeSetup|Boolean||
|relevantRolesSettings|String collection||
|skipSetup|Boolean||
|setupStatus|Enumeration|. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [tenantSetupInfo](../resources/tenantsetupinfo.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_tenantsetupinfo"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.tenantSetupInfo not found
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.tenantSetupInfo",
  "userRolesActions": "User Roles Actions value",
  "firstTimeSetup": true,
  "relevantRolesSettings": [
    "Relevant Roles Settings value"
  ],
  "skipSetup": true,
  "setupStatus": "String"
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
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.tenantSetupInfo",
  "id": "eb5fba04-ba04-eb5f-04ba-5feb04ba5feb",
  "userRolesActions": "User Roles Actions value",
  "firstTimeSetup": true,
  "relevantRolesSettings": [
    "Relevant Roles Settings value"
  ],
  "skipSetup": true,
  "setupStatus": "String"
}
```

