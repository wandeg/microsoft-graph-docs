---
title: "authenticationMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# authenticationMethod resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get authenticationMethod](../api/authenticationmethod-get.md)|[authenticationMethod](../resources/authenticationmethod.md)|Read properties and relationships of the [authenticationMethod](../resources/authenticationmethod.md) object.|
|[enableSmsSignIn](../api/authenticationmethod-enablesmssignin.md)|None||
|[disableSmsSignIn](../api/authenticationmethod-disablesmssignin.md)|None||
|[resetPassword](../api/authenticationmethod-resetpassword.md)|[passwordResetResponse](../resources/passwordresetresponse.md)||
|[List methods](../api/authentication-list-methods.md)|[authenticationMethod](../resources/authenticationmethod.md) collection|Get the authenticationMethods from the methods navigation property.|
|[Add methods](../api/authentication-post-methods.md)|[authenticationMethod](../resources/authenticationmethod.md)|Add methods by posting to the methods collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethod",
  "id": "String (identifier)"
}
```

