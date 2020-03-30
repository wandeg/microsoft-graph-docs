---
title: "Get accessReviewDecision"
description: "Read properties and relationships of the accessReviewDecision object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessReviewDecision

Namespace: microsoft.graph

Read properties and relationships of the [accessReviewDecision](../resources/accessreviewdecision.md) object.

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
GET /accessReviewDecisions/{accessReviewDecisionsId}
GET /accessReviews/{accessReviewsId}/decisions/{accessReviewDecisionId}
GET /accessReviews/{accessReviewsId}/myDecisions/{accessReviewDecisionId}
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/decisions/{accessReviewDecisionId}
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/myDecisions/{accessReviewDecisionId}
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
If successful, this method returns a `200 OK` response code and [accessReviewDecision](../resources/accessreviewdecision.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accessreviewdecision"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviewDecisions/{accessReviewDecisionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 826

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewDecision",
    "id": "34111069-1069-3411-6910-113469101134",
    "accessReviewId": "Access Review Id value",
    "reviewedBy": {
      "@odata.type": "microsoft.graph.userIdentity",
      "id": "Id value",
      "displayName": "Display Name value",
      "ipAddress": "Ip Address value",
      "userPrincipalName": "User Principal Name value"
    },
    "reviewedDateTime": "2016-12-31T23:58:25.6297416+00:00",
    "reviewResult": "Review Result value",
    "justification": "Justification value",
    "appliedBy": {
      "@odata.type": "microsoft.graph.userIdentity"
    },
    "appliedDateTime": "2016-12-31T23:58:02.3117314+00:00",
    "applyResult": "Apply Result value",
    "accessRecommendation": "Access Recommendation value"
  }
}
```

