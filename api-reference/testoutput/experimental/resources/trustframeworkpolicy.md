---
title: "trustFrameworkPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# trustFrameworkPolicy resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trustFrameworkPolicy](../api/trustframeworkpolicy-get.md)|[trustFrameworkPolicy](../resources/trustFrameworkPolicy.md)|Read properties and relationships of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.|
|[Delete trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|None|Deletes a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).|
|[Update trustFrameworkPolicy](../api/trustframeworkpolicy-update.md)|[trustFrameworkPolicy](../resources/trustFrameworkPolicy.md)|Update the properties of a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.|
|[List policies](../api/trustframework-list-policies.md)|[trustFrameworkPolicy](../resources/trustFrameworkPolicy.md) collection|Get the trustFrameworkPolicies from the policies navigation property.|
|[Add policies](../api/trustframework-post-policies.md)|[trustFrameworkPolicy](../resources/trustFrameworkPolicy.md)|Add policies by posting to the policies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trustFrameworkPolicy",
  "id": "String (identifier)"
}
```

