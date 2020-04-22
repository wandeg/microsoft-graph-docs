---
title: "List decisions"
description: "Get the accessReviewDecisions from the decisions navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List decisions

Namespace: microsoft.graph

Get the accessReviewDecisions from the decisions navigation property.

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
GET /accessReviews/{accessReviewsId}/decisions
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
If successful, this method returns a `200 OK` response code and a collection of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accessreviewdecision"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/accessReviews/{accessReviewsId}/decisions
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessreviewdecision)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReviewDecision",
      "id": "1771476e-476e-1771-6e47-71176e477117",
      "accessReviewId": "Access Review Id value",
      "reviewedBy": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "reviewedDateTime": "2017-01-01T00:02:48.7552683+00:00",
      "reviewResult": "Review Result value",
      "justification": "Justification value",
      "appliedBy": {
        "@odata.type": "microsoft.graph.userIdentity"
      },
      "appliedDateTime": "2017-01-01T00:02:32.7701843+00:00",
      "applyResult": "Apply Result value",
      "accessRecommendation": "Access Recommendation value"
    }
  ]
}
```

