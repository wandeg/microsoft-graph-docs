---
title: "request resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# request resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List requests](../api/request-list.md)|[request](../resources/request.md) collection|List properties and relationships of the [request](../resources/request.md) objects.|
|[Get request](../api/request-get.md)|[request](../resources/request.md)|Read properties and relationships of the [request](../resources/request.md) object.|
|[Create request](../api/request-create.md)|[request](../resources/request.md)|Create a new [request](../resources/request.md) object.|
|[Delete request](../api/request-delete.md)|None|Deletes a [request](../resources/request.md).|
|[Update request](../api/request-update.md)|[request](../resources/request.md)|Update the properties of a [request](../resources/request.md) object.|
|[stop](../api/request-stop.md)|None||
|[recordDecisions](../api/request-recorddecisions.md)|None||
|[List decisions](../api/request-list-decisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md) collection|Get the accessReviewDecisions from the decisions navigation property.|
|[Add decisions](../api/request-post-decisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Add decisions by posting to the decisions collection.|
|[List myDecisions](../api/request-list-mydecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md) collection|Get the accessReviewDecisions from the myDecisions navigation property.|
|[Add myDecisions](../api/request-post-mydecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Add myDecisions by posting to the myDecisions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|businessFlowId|String||
|createdBy|[userIdentity](../resources/useridentity.md)||
|customData|String||
|deDuplicationId|String||
|description|String||
|displayName|String||
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|policy|[governancePolicy](../resources/governancepolicy.md)||
|policyTemplateId|String||
|recordVersion|String||
|schemaId|String||
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)||
|startDateTime|DateTimeOffset||
|status|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|decisions|[accessReviewDecision](../resources/accessreviewdecision.md) collection||
|myDecisions|[accessReviewDecision](../resources/accessreviewdecision.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "businessFlowId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "deDuplicationId": "String",
  "schemaId": "String",
  "customData": "String",
  "recordVersion": "String",
  "policyTemplateId": "String",
  "policy": {
    "@odata.type": "microsoft.graph.governancePolicy",
    "decisionMakerCriteria": [
      {
        "@odata.type": "microsoft.graph.groupMembershipGovernanceCriteria",
        "groupId": "String"
      }
    ],
    "notificationPolicy": {
      "@odata.type": "microsoft.graph.governanceNotificationPolicy",
      "notificationTemplates": [
        {
          "@odata.type": "microsoft.graph.governanceNotificationTemplate",
          "type": "String",
          "source": "String",
          "version": "String",
          "culture": "String"
        }
      ],
      "enabledTemplateTypes": [
        "String"
      ]
    }
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings",
    "mailNotificationsEnabled": true,
    "remindersEnabled": true,
    "justificationRequiredOnApproval": true,
    "recurrenceSettings": {
      "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings",
      "recurrenceType": "String",
      "recurrenceEndType": "String",
      "durationInDays": 1024,
      "recurrenceCount": 1024
    },
    "autoReviewEnabled": true,
    "activityDurationInDays": 1024,
    "autoReviewSettings": {
      "@odata.type": "microsoft.graph.autoReviewSettings",
      "notReviewedResult": "String"
    },
    "autoApplyReviewResultsEnabled": true,
    "accessRecommendationsEnabled": true
  }
}
```

