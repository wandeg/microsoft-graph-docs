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
|[List auditEvents](../api/auditevent-list.md)|[auditEvent](../resources/auditevent.md) collection|List properties and relationships of the [auditEvent](../resources/auditevent.md) objects.|
|[Get auditEvent](../api/auditevent-get.md)|[auditEvent](../resources/auditevent.md)|Read properties and relationships of the [auditEvent](../resources/auditevent.md) object.|
|[Create auditEvent](../api/auditevent-create.md)|[auditEvent](../resources/auditevent.md)|Create a new [auditEvent](../resources/auditevent.md) object.|
|[Delete auditEvent](../api/auditevent-delete.md)|None|Deletes a [auditEvent](../resources/auditevent.md).|
|[Update auditEvent](../api/auditevent-update.md)|[auditEvent](../resources/auditevent.md)|Update the properties of a [auditEvent](../resources/auditevent.md) object.|
|[getAuditCategories](../api/auditevent-getauditcategories.md)|String collection||
|[getAuditActivityTypes](../api/auditevent-getauditactivitytypes.md)|String collection||
|[List auditEvents](../api/intune-devices-devicemanagement-list-auditevents.md)|[auditEvent](../resources/auditevent.md) collection|Get the auditEvents from the auditEvents navigation property.|
|[Add auditEvents](../api/intune-devices-devicemanagement-post-auditevents.md)|[auditEvent](../resources/auditevent.md)|Add auditEvents by posting to the auditEvents collection.|

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

## JSON Representation
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

