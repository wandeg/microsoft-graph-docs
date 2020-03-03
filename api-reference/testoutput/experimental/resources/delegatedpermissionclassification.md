---
title: "delegatedPermissionClassification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# delegatedPermissionClassification resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List delegatedPermissionClassifications](../api/delegatedpermissionclassification-list.md)|[delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) collection|List properties and relationships of the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects.|
|[Get delegatedPermissionClassification](../api/delegatedpermissionclassification-get.md)|[delegatedPermissionClassification](../resources/delegatedpermissionclassification.md)|Read properties and relationships of the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.|
|[Create delegatedPermissionClassification](../api/delegatedpermissionclassification-create.md)|[delegatedPermissionClassification](../resources/delegatedpermissionclassification.md)|Create a new [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.|
|[Delete delegatedPermissionClassification](../api/delegatedpermissionclassification-delete.md)|None|Deletes a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md).|
|[Update delegatedPermissionClassification](../api/delegatedpermissionclassification-update.md)|[delegatedPermissionClassification](../resources/delegatedpermissionclassification.md)|Update the properties of a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|Enumeration|. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|permissionId|String||
|permissionName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedPermissionClassification",
  "id": "String (identifier)",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```

