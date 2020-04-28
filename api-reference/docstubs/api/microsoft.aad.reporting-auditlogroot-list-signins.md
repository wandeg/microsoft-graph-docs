---
title: "List signIns"
description: "Get the signIns from the signIns navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List signIns

Namespace: Microsoft.AAD.Reporting

Get the signIns from the signIns navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /auditLogs/signIns
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [signIn](../resources/signin.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_signin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.signin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.signIn",
      "alternateSignInName": "Alternate Sign In Name value",
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "appliedConditionalAccessPolicies": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy",
          "id": "Id value",
          "displayName": "Display Name value",
          "enforcedGrantControls": [
            "Enforced Grant Controls value"
          ],
          "enforcedSessionControls": [
            "Enforced Session Controls value"
          ],
          "conditionsSatisfied": "String",
          "conditionsNotSatisfied": "String",
          "result": "String"
        }
      ],
      "authenticationDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail",
          "authenticationStepDateTime": "2016-12-31T23:59:41.5324069+00:00",
          "authenticationMethod": "Authentication Method value",
          "authenticationMethodDetail": "Authentication Method Detail value",
          "succeeded": true,
          "authenticationStepResultDetail": "Authentication Step Result Detail value",
          "authenticationStepRequirement": "Authentication Step Requirement value"
        }
      ],
      "authenticationMethodsUsed": [
        "Authentication Methods Used value"
      ],
      "authenticationProcessingDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "authenticationRequirementPolicies": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy",
          "requirementProvider": "String",
          "detail": "Detail value"
        }
      ],
      "clientAppUsed": "Client App Used value",
      "conditionalAccessStatus": "String",
      "correlationId": "Correlation Id value",
      "createdDateTime": "2016-12-31T23:59:18.0340888+00:00",
      "deviceDetail": {
        "@odata.type": "Microsoft.AAD.Reporting.deviceDetail",
        "deviceId": "Device Id value",
        "operatingSystem": "Operating System value",
        "browser": "Browser value",
        "browserId": "Browser Id value",
        "isCompliant": true,
        "isManaged": true,
        "trustType": "Trust Type value"
      },
      "id": "97a576cb-76cb-97a5-cb76-a597cb76a597",
      "isInteractive": true,
      "ipAddress": "Ip Address value",
      "location": {
        "@odata.type": "Microsoft.AAD.Reporting.signInLocation",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "geoCoordinates": {
          "@odata.type": "Microsoft.AAD.Reporting.geoCoordinates",
          "altitude": "Double",
          "latitude": "Double",
          "longitude": "Double"
        }
      },
      "mfaDetail": {
        "@odata.type": "Microsoft.AAD.Reporting.mfaDetail",
        "authMethod": "Auth Method value",
        "authDetail": "Auth Detail value"
      },
      "networkLocationDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail",
          "networkType": "String",
          "networkNames": [
            "Network Names value"
          ]
        }
      ],
      "originalRequestId": "Original Request Id value",
      "processingTimeInMilliseconds": 12,
      "riskDetail": "String",
      "riskEventTypes": [
        "String"
      ],
      "riskLevelAggregated": "String",
      "riskLevelDuringSignIn": "String",
      "riskState": "String",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "Resource Id value",
      "servicePrincipalId": "Service Principal Id value",
      "servicePrincipalName": "Service Principal Name value",
      "status": {
        "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
        "errorCode": 9,
        "failureReason": "Failure Reason value",
        "additionalDetails": "Additional Details value"
      },
      "tokenIssuerName": "Token Issuer Name value",
      "tokenIssuerType": "String",
      "userAgent": "User Agent value",
      "userDisplayName": "User Display Name value",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

