---
title: "Create relyingPartyDetailedSummary"
description: "Create a new relyingPartyDetailedSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create relyingPartyDetailedSummary
Namespace: microsoft.graph

Create a new [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

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
POST ** Collection URI for microsoft.graph.relyingPartyDetailedSummary not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

The following table shows the properties that are required when you create the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|relyingPartyId|String|**TODO: Add Description**|
|serviceId|String|**TODO: Add Description**|
|relyingPartyName|String|**TODO: Add Description**|
|successfulSignInCount|Int64|**TODO: Add Description**|
|failedSignInCount|Int64|**TODO: Add Description**|
|totalSignInCount|Int64|**TODO: Add Description**|
|signInSuccessRate|Double|**TODO: Add Description**|
|uniqueUserCount|Int64|**TODO: Add Description**|
|migrationStatus|migrationStatus|**TODO: Add Description**. Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_relyingpartydetailedsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.relyingPartyDetailedSummary not found
Content-Type: application/json
Content-length: 512

{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "relyingPartyId": "String",
  "serviceId": "String",
  "relyingPartyName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "totalSignInCount": "Integer",
  "signInSuccessRate": "Double",
  "uniqueUserCount": "Integer",
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "replyUrls": [
    "String"
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingpartydetailedsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "id": "a104067a-067a-a104-7a06-04a17a0604a1",
  "relyingPartyId": "String",
  "serviceId": "String",
  "relyingPartyName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "totalSignInCount": "Integer",
  "signInSuccessRate": "Double",
  "uniqueUserCount": "Integer",
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "replyUrls": [
    "String"
  ]
}
```

