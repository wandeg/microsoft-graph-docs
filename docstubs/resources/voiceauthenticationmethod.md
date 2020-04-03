---
title: "voiceAuthenticationMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# voiceAuthenticationMethod resource type


Namespace: microsoft.graph




Inherits from [authenticationMethod](../resources/authenticationmethod.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get voiceAuthenticationMethod](../api/voiceauthenticationmethod-get.md)|[voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md)|Read properties and relationships of the [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object.|
|[Update voiceAuthenticationMethod](../api/voiceauthenticationmethod-update.md)|[voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md)|Update the properties of a [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object.|
|[enableSmsSignIn](../api/voiceauthenticationmethod-enablesmssignin.md)|None||
|[disableSmsSignIn](../api/voiceauthenticationmethod-disablesmssignin.md)|None||
|[resetPassword](../api/voiceauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.voiceAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.voiceAuthenticationMethod",
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "String"
}
```

