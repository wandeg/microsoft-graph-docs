---
title: "trustFramework resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trustFramework resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List trustFrameworks](../api/trustframework-list.md)|[trustFramework](../resources/trustframework.md) collection|List properties and relationships of the [trustFramework](../resources/trustframework.md) objects.|
|[Get trustFramework](../api/trustframework-get.md)|[trustFramework](../resources/trustframework.md)|Read properties and relationships of the [trustFramework](../resources/trustframework.md) object.|
|[Create trustFramework](../api/trustframework-create.md)|[trustFramework](../resources/trustframework.md)|Create a new [trustFramework](../resources/trustframework.md) object.|
|[Delete trustFramework](../api/trustframework-delete.md)|None|Deletes a [trustFramework](../resources/trustframework.md).|
|[Update trustFramework](../api/trustframework-update.md)|[trustFramework](../resources/trustframework.md)|Update the properties of a [trustFramework](../resources/trustframework.md) object.|
|[List policies](../api/trustframework-list-policies.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) collection|Get the trustFrameworkPolicies from the policies navigation property.|
|[Add policies](../api/trustframework-post-policies.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)|Add policies by posting to the policies collection.|
|[List keySets](../api/trustframework-list-keysets.md)|[trustFrameworkKeySet](../resources/trustframeworkkeyset.md) collection|Get the trustFrameworkKeySets from the keySets navigation property.|
|[Add keySets](../api/trustframework-post-keysets.md)|[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)|Add keySets by posting to the keySets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|keySets|[trustFrameworkKeySet](../resources/trustframeworkkeyset.md) collection||
|policies|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.trustFramework",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trustFramework",
  "id": "String (identifier)"
}
```

