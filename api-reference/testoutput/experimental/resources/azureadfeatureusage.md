---
title: "azureADFeatureUsage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# azureADFeatureUsage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List azureADFeatureUsages](../api/azureadfeatureusage-list.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|List properties and relationships of the [azureADFeatureUsage](../resources/azureadfeatureusage.md) objects.|
|[Get azureADFeatureUsage](../api/azureadfeatureusage-get.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md)|Read properties and relationships of the [azureADFeatureUsage](../resources/azureadfeatureusage.md) object.|
|[Create azureADFeatureUsage](../api/azureadfeatureusage-create.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md)|Create a new [azureADFeatureUsage](../resources/azureadfeatureusage.md) object.|
|[Delete azureADFeatureUsage](../api/azureadfeatureusage-delete.md)|None|Deletes a [azureADFeatureUsage](../resources/azureadfeatureusage.md).|
|[Update azureADFeatureUsage](../api/azureadfeatureusage-update.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md)|Update the properties of a [azureADFeatureUsage](../resources/azureadfeatureusage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|featureName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|snapshotDateTime|DateTimeOffset||
|usage|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADFeatureUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADFeatureUsage",
  "id": "String (identifier)",
  "snapshotDateTime": "String (timestamp)",
  "featureName": "String",
  "usage": 1024
}
```

