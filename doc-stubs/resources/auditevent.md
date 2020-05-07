---
title: "auditEvent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# auditEvent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getAuditCategories](../api/auditevent-getauditcategories.md)|String collection|**TODO: Add Description**|
|[getAuditActivityTypes](../api/auditevent-getauditactivitytypes.md)|String collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|String|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|activityOperationType|String|**TODO: Add Description**|
|activityResult|String|**TODO: Add Description**|
|activityType|String|**TODO: Add Description**|
|actor|[auditActor](../resources/auditactor.md)|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|componentName|String|**TODO: Add Description**|
|correlationId|Guid|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resources|[auditResource](../resources/auditresource.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource"
    }
  ],
  "category": "String"
}
```

