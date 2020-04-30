---
title: "delegatedPermissionClassification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# delegatedPermissionClassification resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get delegatedPermissionClassification](../api/microsoft.directoryservices-delegatedpermissionclassification-get.md)|[delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md)|Read properties and relationships of a [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md) object.|
|[Update delegatedPermissionClassification](../api/microsoft.directoryservices-delegatedpermissionclassification-update.md)|[delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md)|Update the properties of a [delegatedPermissionClassification](../resources/microsoft.directoryservices-delegatedpermissionclassification.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|permissionClassificationType|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `unknownFutureValue`.|
|id|String|**TODO: Add Description**|
|permissionId|String|**TODO: Add Description**|
|permissionName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.delegatedPermissionClassification",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "id": "String (identifier)",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```

