---
title: "Create passwordMethods"
description: "Create a new passwordMethods object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create passwordMethods

Namespace: microsoft.graph

Create a new passwordMethods object.

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
POST /invitations/{invitationsId}/invitedUser/authentication/passwordMethods
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|password|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_passwordauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/authentication/passwordMethods
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
  "password": "Password value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordauthenticationmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
  "id": "1e73e55b-e55b-1e73-5be5-731e5be5731e",
  "password": "Password value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00"
}
```

