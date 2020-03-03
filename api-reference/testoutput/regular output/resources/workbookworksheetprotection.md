---
title: "workbookWorksheetProtection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookWorksheetProtection resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookWorksheetProtections](../api/workbookworksheetprotection-list.md)|[workbookWorksheetProtection](../resources/workbookWorksheetProtection.md) collection|List properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects.|
|[Get workbookWorksheetProtection](../api/workbookworksheetprotection-get.md)|[workbookWorksheetProtection](../resources/workbookWorksheetProtection.md)|Read properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Create workbookWorksheetProtection](../api/workbookworksheetprotection-create.md)|[workbookWorksheetProtection](../resources/workbookWorksheetProtection.md)|Create a new [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Delete workbookWorksheetProtection](../api/workbookworksheetprotection-delete.md)|None|Deletes a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md).|
|[Update workbookWorksheetProtection](../api/workbookworksheetprotection-update.md)|[workbookWorksheetProtection](../resources/workbookWorksheetProtection.md)|Update the properties of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookWorksheetProtectionOptions.md)||
|protected|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "id": "String (identifier)",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
  },
  "protected": true
}
```

