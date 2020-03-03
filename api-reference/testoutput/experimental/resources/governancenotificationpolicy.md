---
title: "governanceNotificationPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# governanceNotificationPolicy resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|enabledTemplateTypes|String collection||
|notificationTemplates|[governanceNotificationTemplate](../resources/governanceNotificationTemplate.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceNotificationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceNotificationPolicy",
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
```

