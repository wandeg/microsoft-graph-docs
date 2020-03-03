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
|[List identityUserFlows](../api/identityuserflow-list.md)|[identityUserFlow](../resources/identityuserflow.md) collection|List properties and relationships of the [identityUserFlow](../resources/identityuserflow.md) objects.|
|[Get identityUserFlow](../api/identityuserflow-get.md)|[identityUserFlow](../resources/identityuserflow.md)|Read properties and relationships of the [identityUserFlow](../resources/identityuserflow.md) object.|
|[Create identityUserFlow](../api/identityuserflow-create.md)|[identityUserFlow](../resources/identityuserflow.md)|Create a new [identityUserFlow](../resources/identityuserflow.md) object.|
|[Delete identityUserFlow](../api/identityuserflow-delete.md)|None|Deletes a [identityUserFlow](../resources/identityuserflow.md).|
|[Update identityUserFlow](../api/identityuserflow-update.md)|[identityUserFlow](../resources/identityuserflow.md)|Update the properties of a [identityUserFlow](../resources/identityuserflow.md) object.|
|[List userFlows](../api/identitycontainer-list-userflows.md)|[identityUserFlow](../resources/identityuserflow.md) collection|Get the identityUserFlows from the userFlows navigation property.|
|[Add userFlows](../api/identitycontainer-post-userflows.md)|[identityUserFlow](../resources/identityuserflow.md)|Add userFlows by posting to the userFlows collection.|

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

