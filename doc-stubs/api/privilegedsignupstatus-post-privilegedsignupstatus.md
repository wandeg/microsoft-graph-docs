---
title: "Create privilegedSignupStatus"
description: "Create a new privilegedSignupStatus object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedSignupStatus

Namespace: microsoft.graph

Create a new [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.

The following table shows the properties that are required when you create the [privilegedSignupStatus](../resources/privilegedsignupstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRegistered|Boolean|**TODO: Add Description**|
|status|setupStatus|**TODO: Add Description**. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|



## Response

If successful, this method returns a `201 Created` response code and a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedsignupstatus_from_privilegedsignupstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedSignupStatus
Content-Type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "isRegistered": "Boolean",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedsignupstatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "id": "6df5731b-731b-6df5-1b73-f56d1b73f56d",
  "isRegistered": "Boolean",
  "status": "String"
}
```

