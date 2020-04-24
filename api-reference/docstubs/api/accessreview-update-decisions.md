---
title: "Update decisions"
description: "Update the properties of a decisions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update decisions

Namespace: microsoft.graph

Update the properties of a decisions object.

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
PATCH /accessReviews/{accessReviewsId}/decisions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessReviewDecision](../resources/accessreviewdecision.md) object.

The following table shows the properties that are required when you create the [accessReviewDecision](../resources/accessreviewdecision.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|accessReviewId|String|**TODO: Add Description**|
|reviewedBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|reviewedDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewResult|String|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|
|appliedBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|appliedDateTime|DateTimeOffset|**TODO: Add Description**|
|applyResult|String|**TODO: Add Description**|
|accessRecommendation|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [accessReviewDecision](../resources/accessreviewdecision.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_decisions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/decisions
Content-Type: application/json
Content-length: 720

{
  "@odata.type": "#microsoft.graph.accessReviewDecision",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

