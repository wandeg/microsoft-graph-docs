---
title: "evaluateLabelJobResultGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# evaluateLabelJobResultGroup resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|automatic|[evaluateLabelJobResult](../resources/evaluatelabeljobresult.md)||
|recommended|[evaluateLabelJobResult](../resources/evaluatelabeljobresult.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResultGroup",
  "automatic": {
    "@odata.type": "microsoft.graph.evaluateLabelJobResult",
    "sensitivityLabel": {
      "@odata.type": "microsoft.graph.matchingLabel",
      "id": "String",
      "name": "String",
      "displayName": "String",
      "description": "String",
      "toolTip": "String",
      "policyTip": "String",
      "isEndpointProtectionEnabled": true,
      "applicationMode": "String",
      "labelActions": [
        {
          "@odata.type": "microsoft.graph.encryptWithUserDefinedRights",
          "encryptWith": "String",
          "decryptionRightsManagementTemplateId": "String",
          "allowMailForwarding": true,
          "allowAdHocPermissions": true
        }
      ],
      "priority": 1024
    },
    "responsibleSensitiveTypes": [
      {
        "@odata.type": "microsoft.graph.responsibleSensitiveType",
        "rulePackageId": "String",
        "rulePackageType": "String",
        "publisherName": "String"
      }
    ],
    "responsiblePolicy": {
      "@odata.type": "microsoft.graph.responsiblePolicy"
    }
  },
  "recommended": {
    "@odata.type": "microsoft.graph.evaluateLabelJobResult"
  }
}
```

