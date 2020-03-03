---
title: "Update accessReviewDecision"
description: "Update the properties of a accessReviewDecision object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessReviewDecision

Update the properties of a [accessReviewDecision](../resources/accessreviewdecision.md) object.

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
PATCH /accessReviewDecisions/{accessReviewDecisionsId}
PATCH /accessReviews/{accessReviewsId}/decisions/{accessReviewDecisionId}
PATCH /accessReviews/{accessReviewsId}/myDecisions/{accessReviewDecisionId}
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/decisions/{accessReviewDecisionId}
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requests/{requestId}/myDecisions/{accessReviewDecisionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [accessReviewDecision](../resources/accessReviewDecision.md) object.

The following table shows the properties that are required when you create the [accessReviewDecision](../resources/accessreviewdecision.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accessReviewId|String||
|reviewedBy|[userIdentity](../resources/userIdentity.md)||
|reviewedDateTime|DateTimeOffset||
|reviewResult|String||
|justification|String||
|appliedBy|[userIdentity](../resources/userIdentity.md)||
|appliedDateTime|DateTimeOffset||
|applyResult|String||
|accessRecommendation|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessReviewDecision](../resources/accessreviewdecision.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accessreviewdecision"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/accessReviewDecisions/{accessReviewDecisionsId}
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
  "reviewedDateTime": "2016-12-31T23:57:10.8561795+03:00",
  "reviewResult": "Review Result value",
  "justification": "Justification value",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "2016-12-31T23:58:26.0451415+03:00",
  "applyResult": "Apply Result value",
  "accessRecommendation": "Access Recommendation value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 769

{
  "@odata.type": "#microsoft.graph.accessReviewDecision",
  "id": "dac74cd6-4cd6-dac7-d64c-c7dad64cc7da",
  "accessReviewId": "Access Review Id value",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "displayName": "Display Name value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "reviewedDateTime": "2016-12-31T23:57:10.8561795+03:00",
  "reviewResult": "Review Result value",
  "justification": "Justification value",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "2016-12-31T23:58:26.0451415+03:00",
  "applyResult": "Apply Result value",
  "accessRecommendation": "Access Recommendation value"
}
```

