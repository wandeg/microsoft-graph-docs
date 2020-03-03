---
title: "Add restrictedSignIns"
description: "Add restrictedSignIns by posting to the restrictedSignIns collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add restrictedSignIns

Add restrictedSignIns by posting to the restrictedSignIns collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /auditLogs/restrictedSignIns/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the restrictedSignIn object.

The following table shows the properties that are required when you create the restrictedSignIn.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signIn.md)|
|userDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/signIn.md)|
|userId|String| Inherited from [signIn](../resources/signIn.md)|
|appId|String| Inherited from [signIn](../resources/signIn.md)|
|appDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|ipAddress|String| Inherited from [signIn](../resources/signIn.md)|
|status|[signInStatus](../resources/signInStatus.md)| Inherited from [signIn](../resources/signIn.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signIn.md)|
|deviceDetail|[deviceDetail](../resources/deviceDetail.md)| Inherited from [signIn](../resources/signIn.md)|
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [signIn](../resources/signIn.md)|
|correlationId|String| Inherited from [signIn](../resources/signIn.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedConditionalAccessPolicy.md) collection| Inherited from [signIn](../resources/signIn.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signIn.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signIn.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|resourceDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|resourceId|String| Inherited from [signIn](../resources/signIn.md)|
|targetTenantId|Guid||



## Response
If successful, this method returns a `201 Created` response code and a [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_restrictedsignin_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/auditLogs/restrictedSignIns
Content-type: application/json
Content-length: 2019

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "ipAddress": "Ip Address value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "clientAppUsed": "Client App Used value",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
    "deviceId": "Device Id value",
    "displayName": "Display Name value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "correlationId": "Correlation Id value",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
      "id": "Id value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "result": "String"
    }
  ],
  "isInteractive": true,
  "riskDetail": "String",
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "riskEventTypes": [
    "String"
  ],
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "targetTenantId": "dd926948-6948-dd92-4869-92dd486992dd"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedsignin"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2127

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "fe5be58d-e58d-fe5b-8de5-5bfe8de55bfe",
  "createdDateTime": "2016-12-31T23:57:22.3554145+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "ipAddress": "Ip Address value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "clientAppUsed": "Client App Used value",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
    "deviceId": "Device Id value",
    "displayName": "Display Name value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "correlationId": "Correlation Id value",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
      "id": "Id value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "result": "String"
    }
  ],
  "isInteractive": true,
  "riskDetail": "String",
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "riskEventTypes": [
    "String"
  ],
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "targetTenantId": "dd926948-6948-dd92-4869-92dd486992dd"
}
```

