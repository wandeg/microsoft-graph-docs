---
title: "configurationManagerClientHealthState resource type"
description: "Configuration manager client health state"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# configurationManagerClientHealthState resource type


Namespace: microsoft.graph

Configuration manager client health state

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorCode|Int32|Error code for failed state.|
|lastSyncDateTime|DateTimeOffset|Datetime for last sync with configuration manager management point.|
|state|configurationManagerClientState|Current configuration manager client state. Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": "Integer",
  "lastSyncDateTime": "String (timestamp)"
}
```

