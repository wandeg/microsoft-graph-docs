---
title: "completeSetup"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# completeSetup

Namespace: microsoft.graph



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
POST /privilegedSignupStatus/completeSetup
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|tenantSetupInfo|[tenantSetupInfo](../resources/tenantsetupinfo.md)||



## Response
If successful, this action returns a `200 OK` response code and a [roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_completesetup"
}
-->
``` http
POST https://graph.microsoft.com/localtest/privilegedSignupStatus/completeSetup

Content-type: application/json
Content-length: 354

{
  "tenantSetupInfo": {
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
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.rolesuccessstatistics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": [
    {
      "@odata.type": "microsoft.graph.roleSuccessStatistics"
    }
  ]
}
```

