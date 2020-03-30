---
title: "mobileAppTroubleshootingAppUpdateHistory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppTroubleshootingAppUpdateHistory resource type


Namespace: microsoft.graph




Inherits from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset| Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)| Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  }
}
```

