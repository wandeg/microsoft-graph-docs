---
title: "securityBaselineCategoryStateSummary resource type"
description: "The security baseline per category compliance state summary for the security baseline of the account."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# securityBaselineCategoryStateSummary resource type

The security baseline per category compliance state summary for the security baseline of the account.


Inherits from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineCategoryStateSummary](../api/securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/securityBaselineCategoryStateSummary.md)|Read properties and relationships of the [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) object.|
|[Delete securityBaselineCategoryStateSummary](../api/securitybaselinecategorystatesummary-delete.md)|None|Deletes a [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md).|
|[Update securityBaselineCategoryStateSummary](../api/securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/securityBaselineCategoryStateSummary.md)|Update the properties of a [securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictCount|Int32|Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|
|displayName|String|The category name|
|errorCount|Int32|Number of error devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|notApplicableCount|Int32|Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|
|notSecureCount|Int32|Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|
|secureCount|Int32|Number of secure devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|
|unknownCount|Int32|Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary",
  "baseType": "microsoft.graph.securityBaselineStateSummary",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```

