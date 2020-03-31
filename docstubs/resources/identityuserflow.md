---
title: "identityUserFlow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identityUserFlow resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityUserFlow](../api/identityuserflow-get.md)|[identityUserFlow](../resources/identityuserflow.md)|Read properties and relationships of the [identityUserFlow](../resources/identityuserflow.md) object.|
|[Update identityUserFlow](../api/identityuserflow-update.md)|[identityUserFlow](../resources/identityuserflow.md)|Update the properties of a [identityUserFlow](../resources/identityuserflow.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userFlowType|Enumeration| Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Single||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlow",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlow",
  "id": "String (identifier)",
  "userFlowType": "String",
  "userFlowTypeVersion": "Single"
}
```

