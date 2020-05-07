---
title: "credentialUserRegistrationDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# credentialUserRegistrationDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authMethods|registrationAuthMethod collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isCapable|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|isMfaRegistered|Boolean|**TODO: Add Description**|
|isRegistered|Boolean|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "isRegistered": "Boolean",
  "isEnabled": "Boolean",
  "isCapable": "Boolean",
  "isMfaRegistered": "Boolean"
}
```

