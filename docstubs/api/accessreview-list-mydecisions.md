---
title: "List myDecisions"
description: "Get the accessReviewDecisions from the myDecisions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List myDecisions

Namespace: microsoft.graph

Get the accessReviewDecisions from the myDecisions navigation property.

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
GET /accessReviews/{accessReviewsId}/myDecisions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accessreviewdecision"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/myDecisions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessreviewdecision)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 878

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReviewDecision",
      "id": "28d9a86e-a86e-28d9-6ea8-d9286ea8d928",
      "accessReviewId": "Access Review Id value",
      "reviewedBy": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "reviewedDateTime": "2016-12-31T23:58:51.3624401+00:00",
      "reviewResult": "Review Result value",
      "justification": "Justification value",
      "appliedBy": {
        "@odata.type": "microsoft.graph.userIdentity"
      },
      "appliedDateTime": "2016-12-31T23:58:32.8909812+00:00",
      "applyResult": "Apply Result value",
      "accessRecommendation": "Access Recommendation value"
    }
  ]
}
```

