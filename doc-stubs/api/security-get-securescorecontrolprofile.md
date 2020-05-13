---
title: "Get secureScoreControlProfiles"
description: "Read the properties and relationships of a secureScoreControlProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get secureScoreControlProfiles

Namespace: microsoft.graph

Read the properties and relationships of a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.

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
GET /Security/secureScoreControlProfiles
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

If successful, this method returns a `200 OK` response code and a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/Security/secureScoreControlProfiles
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.secureScoreControlProfile",
    "id": "d6c37752-7752-d6c3-5277-c3d65277c3d6",
    "actionType": "String",
    "actionUrl": "String",
    "azureTenantId": "String",
    "complianceInformation": [
      {
        "@odata.type": "microsoft.graph.complianceInformation"
      }
    ],
    "controlCategory": "String",
    "controlStateUpdates": [
      {
        "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
      }
    ],
    "deprecated": "Boolean",
    "implementationCost": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "maxScore": "Double",
    "rank": "Integer",
    "remediation": "String",
    "remediationImpact": "String",
    "service": "String",
    "threats": [
      "String"
    ],
    "tier": "String",
    "title": "String",
    "userImpact": "String",
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation"
    }
  }
}
```

