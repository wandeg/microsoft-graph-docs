---
title: "mobileAppTroubleshootingAppUpdateHistory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppTroubleshootingAppUpdateHistory resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|**TODO: Add Description** Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
  }
}
```

