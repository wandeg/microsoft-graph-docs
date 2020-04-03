---
title: "credentialUserRegistrationDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# credentialUserRegistrationDetails resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get credentialUserRegistrationDetails](../api/credentialuserregistrationdetails-get.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Read properties and relationships of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.|
|[Update credentialUserRegistrationDetails](../api/credentialuserregistrationdetails-update.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Update the properties of a [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethods|Enumeration collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|isCapable|Boolean||
|isEnabled|Boolean||
|isMfaRegistered|Boolean||
|isRegistered|Boolean||
|userDisplayName|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "authMethods": [
    "String"
  ],
  "isRegistered": true,
  "isEnabled": true,
  "isCapable": true,
  "isMfaRegistered": true
}
```

