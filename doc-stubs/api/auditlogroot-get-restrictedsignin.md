---
title: "Get restrictedSignIns"
description: "Read the properties and relationships of a restrictedSignIn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get restrictedSignIns

Namespace: microsoft.graph

Read the properties and relationships of a [restrictedSignIn](../resources/restrictedsignin.md) object.

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

If successful, this method returns a `200 OK` response code and a [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/auditLogs/restrictedSignIns
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedSignIn"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedSignIn",
    "id": "f7568eea-8eea-f756-ea8e-56f7ea8e56f7",
    "createdDateTime": "String (timestamp)",
    "userDisplayName": "String",
    "userPrincipalName": "String",
    "userId": "String",
    "appId": "String",
    "appDisplayName": "String",
    "ipAddress": "String",
    "status": {
      "@odata.type": "microsoft.graph.signInStatus"
    },
    "clientAppUsed": "String",
    "deviceDetail": {
      "@odata.type": "microsoft.graph.deviceDetail"
    },
    "location": {
      "@odata.type": "microsoft.graph.signInLocation"
    },
    "correlationId": "String",
    "conditionalAccessStatus": "String",
    "appliedConditionalAccessPolicies": [
      {
        "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
      }
    ],
    "isInteractive": "Boolean",
    "riskDetail": "String",
    "riskLevelAggregated": "String",
    "riskLevelDuringSignIn": "String",
    "riskState": "String",
    "riskEventTypes": [
      "String"
    ],
    "riskEventTypes_v2": [
      "String"
    ],
    "resourceDisplayName": "String",
    "resourceId": "String",
    "targetTenantId": "Guid"
  }
}
```

