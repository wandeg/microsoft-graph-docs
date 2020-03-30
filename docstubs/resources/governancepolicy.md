---
title: "governancePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governancePolicy resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|decisionMakerCriteria|[governanceCriteria](../resources/governancecriteria.md) collection||
|notificationPolicy|[governanceNotificationPolicy](../resources/governancenotificationpolicy.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governancePolicy",
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
        "id": "String",
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
}
```

