---
title: "passwordAuthenticationMethod resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# passwordAuthenticationMethod resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [authenticationMethod](../resources/authenticationmethod.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Read the properties and relationships of a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[Update passwordAuthenticationMethod](../api/passwordauthenticationmethod-update.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Update the properties of a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[enableSmsSignIn](../api/passwordauthenticationmethod-enablesmssignin.md)|None|**TODO: Add Description**|
|[disableSmsSignIn](../api/passwordauthenticationmethod-disablesmssignin.md)|None|**TODO: Add Description**|
|[resetPassword](../api/passwordauthenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|password|String|**TODO: Add Description**|

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

