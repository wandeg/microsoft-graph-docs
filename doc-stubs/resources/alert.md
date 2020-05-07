---
title: "alert resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# alert resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[updateAlerts](../api/alert-updatealerts.md)|[alert](../resources/alert.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityGroupName|String|**TODO: Add Description**|
|assignedTo|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|category|String|**TODO: Add Description**|
|closedDateTime|DateTimeOffset|**TODO: Add Description**|
|cloudAppStates|[cloudAppSecurityState](../resources/cloudappsecuritystate.md) collection|**TODO: Add Description**|
|comments|String collection|**TODO: Add Description**|
|confidence|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|detectionIds|String collection|**TODO: Add Description**|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|feedback|alertFeedback|**TODO: Add Description**. Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|fileStates|[fileSecurityState](../resources/filesecuritystate.md) collection|**TODO: Add Description**|
|historyStates|[alertHistoryState](../resources/alerthistorystate.md) collection|**TODO: Add Description**|
|hostStates|[hostSecurityState](../resources/hostsecuritystate.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|malwareStates|[malwareState](../resources/malwarestate.md) collection|**TODO: Add Description**|
|networkConnections|[networkConnection](../resources/networkconnection.md) collection|**TODO: Add Description**|
|processes|[process](../resources/process.md) collection|**TODO: Add Description**|
|recommendedActions|String collection|**TODO: Add Description**|
|registryKeyStates|[registryKeyState](../resources/registrykeystate.md) collection|**TODO: Add Description**|
|severity|alertSeverity|**TODO: Add Description**. Possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.|
|sourceMaterials|String collection|**TODO: Add Description**|
|status|alertStatus|**TODO: Add Description**. Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|tags|String collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|triggers|[alertTrigger](../resources/alerttrigger.md) collection|**TODO: Add Description**|
|userStates|[userSecurityState](../resources/usersecuritystate.md) collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alert",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.alert",
  "id": "String (identifier)",
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "@odata.type": "microsoft.graph.cloudAppSecurityState"
    }
  ],
  "comments": [
    "String"
  ],
  "confidence": "Integer",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": [
    "String"
  ],
  "eventDateTime": "String (timestamp)",
  "feedback": "String",
  "fileStates": [
    {
      "@odata.type": "microsoft.graph.fileSecurityState"
    }
  ],
  "historyStates": [
    {
      "@odata.type": "microsoft.graph.alertHistoryState"
    }
  ],
  "hostStates": [
    {
      "@odata.type": "microsoft.graph.hostSecurityState"
    }
  ],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState"
    }
  ],
  "networkConnections": [
    {
      "@odata.type": "microsoft.graph.networkConnection"
    }
  ],
  "processes": [
    {
      "@odata.type": "microsoft.graph.process"
    }
  ],
  "recommendedActions": [
    "String"
  ],
  "registryKeyStates": [
    {
      "@odata.type": "microsoft.graph.registryKeyState"
    }
  ],
  "severity": "String",
  "sourceMaterials": [
    "String"
  ],
  "status": "String",
  "tags": [
    "String"
  ],
  "title": "String",
  "triggers": [
    {
      "@odata.type": "microsoft.graph.alertTrigger"
    }
  ],
  "userStates": [
    {
      "@odata.type": "microsoft.graph.userSecurityState"
    }
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState"
    }
  ]
}
```

