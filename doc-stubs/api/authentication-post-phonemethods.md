---
title: "Create phoneMethods"
description: "Create a new phoneMethods object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create phoneMethods

Namespace: microsoft.graph

Create a new phoneMethods object.

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
POST /users/{usersId}/authentication/phoneMethods
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|phoneNumber|String|**TODO: Add Description**|
|phoneType|authenticationPhoneType|**TODO: Add Description**. Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|smsSignInState|authenticationMethodSignInState|**TODO: Add Description**. Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, `notConfigured`, `unknownFutureValue`.|



## Response

If successful, this method returns a `201 Created` response code and a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/authentication/phoneMethods
Content-Type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "phoneNumber": "String",
  "phoneType": "String",
  "smsSignInState": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneauthenticationmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "eabffa1c-fa1c-eabf-1cfa-bfea1cfabfea",
  "phoneNumber": "String",
  "phoneType": "String",
  "smsSignInState": "String"
}
```

