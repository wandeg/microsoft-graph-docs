---
title: "deviceHealthScriptRemediationHistory resource type"
description: "The number of devices remediated by a device health script on a given date with the last modified time."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptRemediationHistory resource type


Namespace: microsoft.graph

The number of devices remediated by a device health script on a given date with the last modified time.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|historyData|[deviceHealthScriptRemediationHistoryData](../resources/devicehealthscriptremediationhistorydata.md) collection|The number of devices remediated by the device health script on the given date.|
|lastModifiedDateTime|DateTimeOffset|The date on which the results history is calculated for the healthscript.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.management.services.api.deviceHealthScriptRemediationHistoryData"
    }
  ]
}
```

