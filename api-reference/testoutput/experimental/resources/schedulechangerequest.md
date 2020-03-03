---
title: "scheduleChangeRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# scheduleChangeRequest resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List scheduleChangeRequests](../api/schedulechangerequest-list.md)|[scheduleChangeRequest](../resources/scheduleChangeRequest.md) collection|List properties and relationships of the [scheduleChangeRequest](../resources/schedulechangerequest.md) objects.|
|[Get scheduleChangeRequest](../api/schedulechangerequest-get.md)|[scheduleChangeRequest](../resources/scheduleChangeRequest.md)|Read properties and relationships of the [scheduleChangeRequest](../resources/schedulechangerequest.md) object.|
|[approve](../api/schedulechangerequest-approve.md)|None||
|[decline](../api/schedulechangerequest-decline.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|Enumeration|. Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|managerActionDateTime|DateTimeOffset||
|managerActionMessage|String||
|managerUserId|String||
|senderDateTime|DateTimeOffset||
|senderMessage|String||
|senderUserId|String||
|state|Enumeration|. Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.scheduleChangeRequest",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleChangeRequest",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "String",
  "senderDateTime": "String (timestamp)",
  "managerActionMessage": "String",
  "managerActionDateTime": "String (timestamp)",
  "senderUserId": "String",
  "managerUserId": "String"
}
```

