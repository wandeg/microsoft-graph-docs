---
title: "mobileAppTroubleshootingAppPolicyCreationHistory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppTroubleshootingAppPolicyCreationHistory resource type


Namespace: microsoft.graph




Inherits from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorCode|String||
|occurrenceDateTime|DateTimeOffset| Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|
|runState|Enumeration| Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)| Inherited from [mobileAppTroubleshootingHistoryItem](../resources/mobileapptroubleshootinghistoryitem.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
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
  },
  "runState": "String",
  "errorCode": "String"
}
```

