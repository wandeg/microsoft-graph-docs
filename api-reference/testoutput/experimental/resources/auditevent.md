---
title: "auditEvent resource type"
description: "A class containing the properties for Audit Event."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# auditEvent resource type


Namespace: microsoft.graph

A class containing the properties for Audit Event.


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
|activity|String|Friendly name of the activity.|
|activityDateTime|DateTimeOffset|The date time in UTC when the activity was performed.|
|activityOperationType|String|The HTTP operation type of the activity.|
|activityResult|String|The result of the activity.|
|activityType|String|The type of activity that was being performed.|
|actor|[auditActor](../resources/auditactor.md)|AAD user and application that are associated with the audit event.|
|category|String|Audit category.|
|componentName|String|Component name.|
|correlationId|Guid|The client request Id that is used to correlate activity within the system.|
|displayName|String|Event display name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|resources|[auditResource](../resources/auditresource.md) collection|Resources being modified.|

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

