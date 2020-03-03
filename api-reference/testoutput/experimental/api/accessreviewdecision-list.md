---
title: "List accessReviewDecisions"
description: "List properties and relationships of the accessReviewDecision objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessReviewDecisions

Namespace: microsoft.graph

List properties and relationships of the [accessReviewDecision](../resources/accessreviewdecision.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /accessReviewDecisions
GET /accessReviews/{accessReviewsId}/decisions
GET /accessReviews/{accessReviewsId}/myDecisions
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/decisions
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/myDecisions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accessreviewdecision"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessReviewDecisions
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
      "id": "903da73c-a73c-903d-3ca7-3d903ca73d90",
      "accessReviewId": "Access Review Id value",
      "reviewedBy": {
        "@odata.type": "microsoft.graph.userIdentity",
        "id": "Id value",
        "displayName": "Display Name value",
        "ipAddress": "Ip Address value",
        "userPrincipalName": "User Principal Name value"
      },
      "reviewedDateTime": "2017-01-01T00:02:24.4487531+03:00",
      "reviewResult": "Review Result value",
      "justification": "Justification value",
      "appliedBy": {
        "@odata.type": "microsoft.graph.userIdentity"
      },
      "appliedDateTime": "2017-01-01T00:01:12.8088916+03:00",
      "applyResult": "Apply Result value",
      "accessRecommendation": "Access Recommendation value"
    }
  ]
}
```

