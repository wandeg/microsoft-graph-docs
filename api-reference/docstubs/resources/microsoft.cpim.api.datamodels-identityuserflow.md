---
title: "identityUserFlow resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# identityUserFlow resource type


Namespace: microsoft.cpim.api.dataModels

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityUserFlow](../api/microsoft.cpim.api.datamodels-identityuserflow-get.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md)|Read properties and relationships of an [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object.|
|[Update identityUserFlow](../api/microsoft.cpim.api.datamodels-identityuserflow-update.md)|[identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md)|Update the properties of a [identityUserFlow](../resources/microsoft.cpim.api.datamodels-identityuserflow.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|userFlowType|userFlowType|**TODO: Add Description**. Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Single|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.cpim.api.dataModels.identityUserFlow",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.cpim.api.dataModels.identityUserFlow",
  "id": "String (identifier)",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

