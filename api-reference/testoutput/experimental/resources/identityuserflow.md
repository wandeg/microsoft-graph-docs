---
title: "identityUserFlow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# identityUserFlow resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get identityUserFlow](../api/identityuserflow-get.md)|[identityUserFlow](../resources/identityUserFlow.md)|Read properties and relationships of the [identityUserFlow](../resources/identityuserflow.md) object.|
|[Delete identityUserFlow](../api/identityuserflow-delete.md)|None|Deletes a [identityUserFlow](../resources/identityuserflow.md).|
|[Update identityUserFlow](../api/identityuserflow-update.md)|[identityUserFlow](../resources/identityUserFlow.md)|Update the properties of a [identityUserFlow](../resources/identityuserflow.md) object.|
|[List userFlows](../api/identitycontainer-list-userflows.md)|[identityUserFlow](../resources/identityUserFlow.md) collection|Get the identityUserFlows from the userFlows navigation property.|
|[Add userFlows](../api/identitycontainer-post-userflows.md)|[identityUserFlow](../resources/identityUserFlow.md)|Add userFlows by posting to the userFlows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userFlowType|Enumeration|. Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Single||

## Relationships
None

## JSON Representation
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

