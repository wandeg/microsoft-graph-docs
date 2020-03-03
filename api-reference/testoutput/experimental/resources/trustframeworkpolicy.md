---
title: "trustFrameworkPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trustFrameworkPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List trustFrameworkPolicies](../api/trustframeworkpolicy-list.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) collection|List properties and relationships of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects.|
|[Get trustFrameworkPolicy](../api/trustframeworkpolicy-get.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)|Read properties and relationships of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.|
|[Create trustFrameworkPolicy](../api/trustframeworkpolicy-create.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)|Create a new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.|
|[Delete trustFrameworkPolicy](../api/trustframeworkpolicy-delete.md)|None|Deletes a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).|
|[Update trustFrameworkPolicy](../api/trustframeworkpolicy-update.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)|Update the properties of a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.|
|[List policies](../api/trustframework-list-policies.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md) collection|Get the trustFrameworkPolicies from the policies navigation property.|
|[Add policies](../api/trustframework-post-policies.md)|[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)|Add policies by posting to the policies collection.|

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

