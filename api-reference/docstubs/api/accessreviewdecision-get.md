---
title: "Get accessReviewDecision"
description: "Read the properties and relationships of an accessReviewDecision object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get accessReviewDecision

Namespace: microsoft.graph

Read the properties and relationships of an [accessReviewDecision](../resources/accessreviewdecision.md) object.

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
GET /accessReviewDecisions/{accessReviewDecisionsId}
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
If successful, this method returns a `200 OK` response code and an [accessReviewDecision](../resources/accessreviewdecision.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accessreviewdecision"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviewDecisions/{accessReviewDecisionsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewDecision",
    "id": "96664958-4958-9666-5849-669658496696",
    "accessReviewId": "Access Review Id value",
    "reviewedBy": {
      "@odata.type": "microsoft.graph.userIdentity",
      "id": "Id value",
      "displayName": "Display Name value",
      "ipAddress": "Ip Address value",
      "userPrincipalName": "User Principal Name value"
    },
    "reviewedDateTime": "2016-12-31T23:58:44.4686785+03:00",
    "reviewResult": "Review Result value",
    "justification": "Justification value",
    "appliedBy": {
      "@odata.type": "microsoft.graph.userIdentity"
    },
    "appliedDateTime": "2016-12-31T23:57:42.9026405+03:00",
    "applyResult": "Apply Result value",
    "accessRecommendation": "Access Recommendation value"
  }
}
```

