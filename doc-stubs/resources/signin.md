---
title: "signIn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# signIn resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List signIns](../api/signin-list.md)|[signIn](../resources/signin.md) collection|Get a list of the [signIn](../resources/signin.md) objects and their properties.|
|[Create signIn](../api/signin-create.md)|[signIn](../resources/signin.md)|Create a new [signIn](../resources/signin.md) object.|
|[Get signIn](../api/signin-get.md)|[signIn](../resources/signin.md)|Read the properties and relationships of a [signIn](../resources/signin.md) object.|
|[Update signIn](../api/signin-update.md)|[signIn](../resources/signin.md)|Update the properties of a [signIn](../resources/signin.md) object.|
|[Delete signIn](../api/signin-delete.md)|None|Deletes a [signIn](../resources/signin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection|**TODO: Add Description**|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection|**TODO: Add Description**|
|authenticationMethodsUsed|String collection|**TODO: Add Description**|
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection|**TODO: Add Description**|
|authenticationRequirement|String|**TODO: Add Description**|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection|**TODO: Add Description**|
|clientAppUsed|String|**TODO: Add Description**|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description**. Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ipAddress|String|**TODO: Add Description**|
|isInteractive|Boolean|**TODO: Add Description**|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description**|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)|**TODO: Add Description**|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection|**TODO: Add Description**|
|originalRequestId|String|**TODO: Add Description**|
|processingTimeInMilliseconds|Int32|**TODO: Add Description**|
|resourceDisplayName|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|riskDetail|riskDetail|**TODO: Add Description**. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description**|
|riskEventTypes_v2|String collection|**TODO: Add Description**|
|riskLevelAggregated|riskLevel|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description**. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String|**TODO: Add Description**|
|servicePrincipalName|String|**TODO: Add Description**|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description**|
|tokenIssuerName|String|**TODO: Add Description**|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description**. Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signIn",
  "id": "String (identifier)",
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "isInteractive": "Boolean",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String"
}
```

