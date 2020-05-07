---
title: "phoneAuthenticationMethod resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# phoneAuthenticationMethod resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [authenticationMethod](../resources/authenticationmethod.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[enableSmsSignIn](../api/phoneauthenticationmethod-enablesmssignin.md)|None|**TODO: Add Description**|
|[disableSmsSignIn](../api/phoneauthenticationmethod-disablesmssignin.md)|None|**TODO: Add Description**|
|[resetPassword](../api/phoneauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)|**TODO: Add Description**|
|[List phoneMethods](../api/authentication-list-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection|Get the phoneAuthenticationMethods from the phoneMethods navigation property.|
|[Create phoneMethods](../api/authentication-post-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Create a new phoneMethods object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|phoneNumber|String|**TODO: Add Description**|
|phoneType|authenticationPhoneType|**TODO: Add Description**. Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|smsSignInState|authenticationMethodSignInState|**TODO: Add Description**. Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, `notConfigured`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "String",
  "smsSignInState": "String"
}
```

