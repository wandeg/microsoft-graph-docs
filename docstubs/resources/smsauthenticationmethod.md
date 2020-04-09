---
title: "smsAuthenticationMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# smsAuthenticationMethod resource type


Namespace: microsoft.graph




Inherits from [authenticationMethod](../resources/authenticationmethod.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get smsAuthenticationMethod](../api/smsauthenticationmethod-get.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md)|Read properties and relationships of the [smsAuthenticationMethod](../resources/smsauthenticationmethod.md) object.|
|[Update smsAuthenticationMethod](../api/smsauthenticationmethod-update.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md)|Update the properties of a [smsAuthenticationMethod](../resources/smsauthenticationmethod.md) object.|
|[enableSmsSignIn](../api/smsauthenticationmethod-enablesmssignin.md)|None||
|[disableSmsSignIn](../api/smsauthenticationmethod-disablesmssignin.md)|None||
|[resetPassword](../api/smsauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)||
|[List smsMethods](../api/authentication-list-smsmethods.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md) collection|Get the smsAuthenticationMethods from the smsMethods navigation property.|
|[Add smsMethods](../api/authentication-post-smsmethods.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md)|Add smsMethods by posting to the smsMethods collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|signInState|Enumeration| Possible values are: `notSupported`, `notAllowedByPolicy`, `notProvisioned`, `phoneNumberCollision`, `provisioned`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethod",
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "String",
  "signInState": "String"
}
```

