---
title: "riskDetection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# riskDetection resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List riskDetections](../api/riskdetection-list.md)|[riskDetection](../resources/riskdetection.md) collection|List properties and relationships of the [riskDetection](../resources/riskdetection.md) objects.|
|[Get riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Read properties and relationships of the [riskDetection](../resources/riskdetection.md) object.|
|[Create riskDetection](../api/riskdetection-post-riskdetections.md)|[riskDetection](../resources/riskdetection.md)|Create a new [riskDetection](../resources/riskdetection.md) object.|
|[Delete riskDetection](../api/riskdetection-delete.md)|None|Deletes a [riskDetection](../resources/riskdetection.md).|
|[Update riskDetection](../api/riskdetection-update.md)|[riskDetection](../resources/riskdetection.md)|Update the properties of a [riskDetection](../resources/riskdetection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration|. Possible values are: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset||
|additionalInfo|String||
|correlationId|String||
|detectedDateTime|DateTimeOffset||
|detectionTimingType|Enumeration|. Possible values are: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String||
|lastUpdatedDateTime|DateTimeOffset||
|location|[signInLocation](../resources/signinlocation.md)||
|requestId|String||
|riskDetail|Enumeration|. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLevel|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration|. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskType|Enumeration|. Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|source|String||
|tokenIssuerType|Enumeration|. Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```

