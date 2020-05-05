---
title: "List restrictedSignIns"
description: "Get the restrictedSignIns from the restrictedSignIns navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List restrictedSignIns

Namespace: Microsoft.AAD.Reporting

Get the restrictedSignIns from the restrictedSignIns navigation property.

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
GET /auditLogs/restrictedSignIns
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [restrictedSignIn](../resources/restrictedsignin.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.restrictedsignin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.restrictedSignIn",
      "alternateSignInName": "String",
      "appDisplayName": "String",
      "appId": "String",
      "appliedConditionalAccessPolicies": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy"
        }
      ],
      "authenticationDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail"
        }
      ],
      "authenticationMethodsUsed": [
        "String"
      ],
      "authenticationProcessingDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.keyValue"
        }
      ],
      "authenticationRequirementPolicies": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy"
        }
      ],
      "clientAppUsed": "String",
      "conditionalAccessStatus": "String",
      "correlationId": "String",
      "createdDateTime": "String (timestamp)",
      "deviceDetail": {
        "@odata.type": "Microsoft.AAD.Reporting.deviceDetail"
      },
      "id": "ea2f1f97-1f97-ea2f-971f-2fea971f2fea",
      "isInteractive": "Boolean",
      "ipAddress": "String",
      "location": {
        "@odata.type": "Microsoft.AAD.Reporting.signInLocation"
      },
      "mfaDetail": {
        "@odata.type": "Microsoft.AAD.Reporting.mfaDetail"
      },
      "networkLocationDetails": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail"
        }
      ],
      "originalRequestId": "String",
      "processingTimeInMilliseconds": "Integer",
      "riskDetail": "String",
      "riskEventTypes": [
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
        "@odata.type": "Microsoft.AAD.Reporting.signInStatus"
      },
      "tokenIssuerName": "String",
      "tokenIssuerType": "String",
      "userAgent": "String",
      "userDisplayName": "String",
      "userId": "String",
      "userPrincipalName": "String",
      "targetTenantId": "Guid"
    }
  ]
}
```

