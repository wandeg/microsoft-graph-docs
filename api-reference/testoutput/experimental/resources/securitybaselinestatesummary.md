---
title: "securityBaselineStateSummary resource type"
description: "The security baseline compliance state summary for the security baseline of the account."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# securityBaselineStateSummary resource type

The security baseline compliance state summary for the security baseline of the account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List securityBaselineStateSummaries](../api/securitybaselinestatesummary-list.md)|[securityBaselineStateSummary](../resources/securityBaselineStateSummary.md) collection|List properties and relationships of the [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) objects.|
|[Get securityBaselineStateSummary](../api/securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|Read properties and relationships of the [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.|
|[Create securityBaselineStateSummary](../api/securitybaselinestatesummary-create.md)|[securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|Create a new [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.|
|[Delete securityBaselineStateSummary](../api/securitybaselinestatesummary-delete.md)|None|Deletes a [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md).|
|[Update securityBaselineStateSummary](../api/securitybaselinestatesummary-update.md)|[securityBaselineStateSummary](../resources/securityBaselineStateSummary.md)|Update the properties of a [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conflictCount|Int32|Number of conflict devices|
|errorCount|Int32|Number of error devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|notApplicableCount|Int32|Number of not applicable devices|
|notSecureCount|Int32|Number of not secure devices|
|secureCount|Int32|Number of secure devices|
|unknownCount|Int32|Number of unknown devices|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```

