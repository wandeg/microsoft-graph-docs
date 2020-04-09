---
title: "passwordAuthenticationMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# passwordAuthenticationMethod resource type


Namespace: microsoft.graph




Inherits from [authenticationMethod](../resources/authenticationmethod.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Read properties and relationships of the [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[Update passwordAuthenticationMethod](../api/passwordauthenticationmethod-update.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Update the properties of a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[enableSmsSignIn](../api/passwordauthenticationmethod-enablesmssignin.md)|None||
|[disableSmsSignIn](../api/passwordauthenticationmethod-disablesmssignin.md)|None||
|[resetPassword](../api/passwordauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)||
|[List passwordMethods](../api/authentication-list-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection|Get the passwordAuthenticationMethods from the passwordMethods navigation property.|
|[Add passwordMethods](../api/authentication-post-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Add passwordMethods by posting to the passwordMethods collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|password|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
  "id": "String (identifier)",
  "password": "String",
  "creationDateTime": "String (timestamp)"
}
```

