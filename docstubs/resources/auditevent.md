---
title: "auditEvent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditEvent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get auditEvent](../api/auditevent-get.md)|[auditEvent](../resources/auditevent.md)|Read properties and relationships of the [auditEvent](../resources/auditevent.md) object.|
|[Update auditEvent](../api/auditevent-update.md)|[auditEvent](../resources/auditevent.md)|Update the properties of a [auditEvent](../resources/auditevent.md) object.|
|[getAuditCategories](../api/auditevent-getauditcategories.md)|String collection||
|[getAuditActivityTypes](../api/auditevent-getauditactivitytypes.md)|String collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|String||
|activityDateTime|DateTimeOffset||
|activityOperationType|String||
|activityResult|String||
|activityType|String||
|actor|[auditActor](../resources/auditactor.md)||
|category|String||
|componentName|String||
|correlationId|Guid||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resources|[auditResource](../resources/auditresource.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

