---
title: "workbookWorksheetProtection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookWorksheetProtection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[protect](../api/workbookworksheetprotection-protect.md)|None|**TODO: Add Description**|
|[unprotect](../api/workbookworksheetprotection-unprotect.md)|None|**TODO: Add Description**|
|[List protection](../api/workbookworksheet-list-protection.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md) collection|Get the workbookWorksheetProtections from the protection navigation property.|
|[Create protection](../api/workbookworksheet-post-protection.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Create a new protection object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookworksheetprotectionoptions.md)|**TODO: Add Description**|
|protected|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "protected": "Boolean"
}
```

