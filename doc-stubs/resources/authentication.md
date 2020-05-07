---
title: "authentication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# authentication resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List methods](../api/authentication-list-methods.md)|[authenticationMethod](../resources/authenticationmethod.md) collection|Get the authenticationMethods from the methods navigation property.|
|[Create methods](../api/authentication-post-methods.md)|[authenticationMethod](../resources/authenticationmethod.md)|Create a new methods object.|
|[Delete methods](../api/authentication-delete-methods.md)|None|Delete a [authenticationMethod](../resources/authenticationmethod.md) object.|
|[Update methods](../api/authentication-update-methods.md)|[authenticationMethod](../resources/authenticationmethod.md)|Update the properties of a methods object.|
|[Get authenticationMethod](../api/authenticationmethod-get.md)|[authenticationMethod](../resources/authenticationmethod.md)|Read the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.|
|[List phoneMethods](../api/authentication-list-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection|Get the phoneAuthenticationMethods from the phoneMethods navigation property.|
|[Create phoneMethods](../api/authentication-post-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Create a new phoneMethods object.|
|[Delete phoneMethods](../api/authentication-delete-phonemethods.md)|None|Delete a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.|
|[Update phoneMethods](../api/authentication-update-phonemethods.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Update the properties of a phoneMethods object.|
|[Get phoneAuthenticationMethod](../api/phoneauthenticationmethod-get.md)|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Read the properties and relationships of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.|
|[List passwordMethods](../api/authentication-list-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection|Get the passwordAuthenticationMethods from the passwordMethods navigation property.|
|[Create passwordMethods](../api/authentication-post-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Create a new passwordMethods object.|
|[Delete passwordMethods](../api/authentication-delete-passwordmethods.md)|None|Delete a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[Update passwordMethods](../api/authentication-update-passwordmethods.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Update the properties of a passwordMethods object.|
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md)|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)|Read the properties and relationships of a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.|
|[List operations](../api/authentication-list-operations.md)|[longRunningOperation](../resources/longrunningoperation.md) collection|Get the longRunningOperations from the operations navigation property.|
|[Create operations](../api/authentication-post-operations.md)|[longRunningOperation](../resources/longrunningoperation.md)|Create a new operations object.|
|[Delete operations](../api/authentication-delete-operations.md)|None|Delete an [longRunningOperation](../resources/longrunningoperation.md) object.|
|[Update operations](../api/authentication-update-operations.md)|[longRunningOperation](../resources/longrunningoperation.md)|Update the properties of an operations object.|
|[Get longRunningOperation](../api/longrunningoperation-get.md)|[longRunningOperation](../resources/longrunningoperation.md)|Read the properties and relationships of a [longRunningOperation](../resources/longrunningoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|methods|[authenticationMethod](../resources/authenticationmethod.md) collection|**TODO: Add Description**|
|operations|[longRunningOperation](../resources/longrunningoperation.md) collection|**TODO: Add Description**|
|passwordMethods|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection|**TODO: Add Description**|
|phoneMethods|[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

