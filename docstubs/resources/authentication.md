---
title: "authentication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authentication resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get authentication](../api/authentication-get.md)|[authentication](../resources/authentication.md)|Read properties and relationships of the [authentication](../resources/authentication.md) object.|
|[Update authentication](../api/authentication-update.md)|[authentication](../resources/authentication.md)|Update the properties of a [authentication](../resources/authentication.md) object.|
|[List methods](../api/authentication-list-methods.md)|[authenticationMethod](../resources/authenticationmethod.md) collection|Get the authenticationMethods from the methods navigation property.|
|[Add methods](../api/authentication-post-methods.md)|[authenticationMethod](../resources/authenticationmethod.md)|Add methods by posting to the methods collection.|
|[List smsMethods](../api/authentication-list-smsmethods.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md) collection|Get the smsAuthenticationMethods from the smsMethods navigation property.|
|[Add smsMethods](../api/authentication-post-smsmethods.md)|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md)|Add smsMethods by posting to the smsMethods collection.|
|[List voiceMethods](../api/authentication-list-voicemethods.md)|[voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) collection|Get the voiceAuthenticationMethods from the voiceMethods navigation property.|
|[Add voiceMethods](../api/authentication-post-voicemethods.md)|[voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md)|Add voiceMethods by posting to the voiceMethods collection.|
|[List phoneMethods](../api/authentication-list-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection|Get the phoneAuthenticationMethods from the phoneMethods navigation property.|
|[Add phoneMethods](../api/authentication-post-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Add phoneMethods by posting to the phoneMethods collection.|
|[List passwordMethods](../api/authentication-list-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection|Get the passwordAuthenticationMethods from the passwordMethods navigation property.|
|[Add passwordMethods](../api/authentication-post-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Add passwordMethods by posting to the passwordMethods collection.|
|[List operations](../api/authentication-list-operations.md)|[longRunningOperation](../resources/longrunningoperation.md) collection|Get the longRunningOperations from the operations navigation property.|
|[Add operations](../api/authentication-post-operations.md)|[longRunningOperation](../resources/longrunningoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|methods|[authenticationMethod](../resources/authenticationmethod.md) collection||
|operations|[longRunningOperation](../resources/longrunningoperation.md) collection||
|passwordMethods|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection||
|phoneMethods|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection||
|smsMethods|[smsAuthenticationMethod](../resources/smsauthenticationmethod.md) collection||
|voiceMethods|[voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authentication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authentication",
  "id": "String (identifier)"
}
```

