---
title: "Add decisions"
description: "Add decisions by posting to the decisions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add decisions

Namespace: microsoft.graph

Add decisions by posting to the decisions collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /accessReviews/{accessReviewsId}/decisions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessReviewDecision](../resources/accessreviewdecision.md) object.

The following table shows the properties that are required when you create the [accessReviewDecision](../resources/accessreviewdecision.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accessReviewId|String||
|reviewedBy|[userIdentity](../resources/useridentity.md)||
|reviewedDateTime|DateTimeOffset||
|reviewResult|String||
|justification|String||
|appliedBy|[userIdentity](../resources/useridentity.md)||
|appliedDateTime|DateTimeOffset||
|applyResult|String||
|accessRecommendation|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessReviewDecision](../resources/accessreviewdecision.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accessreviewdecision_from_accessreviewdecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/decisions
Content-type: application/json
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
  "reviewedDateTime": "2016-12-31T23:58:30.2620034+00:00",
  "reviewResult": "Review Result value",
  "justification": "Justification value",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "2017-01-01T00:00:22.6764666+00:00",
  "applyResult": "Apply Result value",
  "accessRecommendation": "Access Recommendation value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessreviewdecision"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 769

{
  "@odata.type": "#microsoft.graph.accessReviewDecision",
  "id": "9bb464da-64da-9bb4-da64-b49bda64b49b",
  "accessReviewId": "Access Review Id value",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "displayName": "Display Name value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "reviewedDateTime": "2016-12-31T23:58:30.2620034+00:00",
  "reviewResult": "Review Result value",
  "justification": "Justification value",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "2017-01-01T00:00:22.6764666+00:00",
  "applyResult": "Apply Result value",
  "accessRecommendation": "Access Recommendation value"
}
```

