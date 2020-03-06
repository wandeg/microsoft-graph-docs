---
title: "evaluateLabelsAndPoliciesResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# evaluateLabelsAndPoliciesResult resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|classificationResult|[detectedSensitiveContentWrapper](../resources/detectedsensitivecontentwrapper.md)||
|dataLossPreventionPoliciesResult|[dlpPoliciesJobResult](../resources/dlppoliciesjobresult.md)||
|sensitivityLabelsResult|[evaluateLabelJobResultGroup](../resources/evaluatelabeljobresultgroup.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesResult",
  "sensitivityLabelsResult": {
    "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup",
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
  },
  "dataLossPreventionPoliciesResult": {
    "@odata.type": "microsoft.graph.dlpPoliciesJobResult",
    "matchingRules": [
      {
        "@odata.type": "microsoft.graph.matchingDlpRule",
        "ruleId": "String",
        "ruleName": "String",
        "policyId": "String",
        "policyName": "String",
        "isMostRestrictive": true,
        "actions": [
          {
            "@odata.type": "microsoft.graph.dlpActionInfo",
            "action": "String"
          }
        ],
        "ruleMode": "String"
      }
    ]
  },
  "classificationResult": {
    "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper",
    "classification": [
      {
        "@odata.type": "microsoft.graph.detectedSensitiveContent",
        "id": "Guid",
        "uniqueCount": 1024,
        "confidence": 1024,
        "recommendedConfidence": 1024,
        "matches": [
          {
            "@odata.type": "microsoft.graph.sensitiveContentLocation",
            "idMatch": "String",
            "offset": 1024,
            "length": 1024,
            "evidences": [
              {
                "@odata.type": "microsoft.graph.sensitiveContentEvidence",
                "match": "String"
              }
            ]
          }
        ]
      }
    ]
  }
}
```

