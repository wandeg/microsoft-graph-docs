---
title: "outlookTask resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# outlookTask resource type


Namespace: microsoft.graph




Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List outlookTasks](../api/outlooktask-list.md)|[outlookTask](../resources/outlooktask.md) collection|List properties and relationships of the [outlookTask](../resources/outlooktask.md) objects.|
|[Get outlookTask](../api/outlooktask-get.md)|[outlookTask](../resources/outlooktask.md)|Read properties and relationships of the [outlookTask](../resources/outlooktask.md) object.|
|[Create outlookTask](../api/outlooktask-create.md)|[outlookTask](../resources/outlooktask.md)|Create a new [outlookTask](../resources/outlooktask.md) object.|
|[Delete outlookTask](../api/outlooktask-delete.md)|None|Deletes a [outlookTask](../resources/outlooktask.md).|
|[Update outlookTask](../api/outlooktask-update.md)|[outlookTask](../resources/outlooktask.md)|Update the properties of a [outlookTask](../resources/outlooktask.md) object.|
|[complete](../api/outlooktask-complete.md)|[outlookTask](../resources/outlooktask.md) collection||
|[List singleValueExtendedProperties](../api/outlooktask-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/outlooktask-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/outlooktask-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/outlooktask-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/outlooktask-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/outlooktask-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|String||
|body|[itemBody](../resources/itembody.md)||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|hasAttachments|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|isReminderOn|Boolean||
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|owner|String||
|parentFolderId|String||
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|sensitivity|Enumeration|. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|status|Enumeration|. Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookTask",
  "baseType": "microsoft.graph.outlookItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookTask",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "assignedTo": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "hasAttachments": true,
  "importance": "String",
  "isReminderOn": true,
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 1024,
      "month": 1024,
      "dayOfMonth": 1024,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "String",
      "numberOfOccurrences": 1024
    }
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "sensitivity": "String",
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "subject": "String"
}
```

