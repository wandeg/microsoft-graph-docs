---
title: "phoneAuthenticationMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# phoneAuthenticationMethod resource type


Namespace: microsoft.graph




Inherits from [authenticationMethod](../resources/authenticationmethod.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get phoneAuthenticationMethod](../api/phoneauthenticationmethod-get.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Read properties and relationships of the [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.|
|[Update phoneAuthenticationMethod](../api/phoneauthenticationmethod-update.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Update the properties of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.|
|[enableSmsSignIn](../api/phoneauthenticationmethod-enablesmssignin.md)|None||
|[disableSmsSignIn](../api/phoneauthenticationmethod-disablesmssignin.md)|None||
|[resetPassword](../api/phoneauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)||
|[List phoneMethods](../api/authentication-list-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection|Get the phoneAuthenticationMethods from the phoneMethods navigation property.|
|[Add phoneMethods](../api/authentication-post-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Add phoneMethods by posting to the phoneMethods collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|smsSignInState|Enumeration| Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, `notConfigured`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

