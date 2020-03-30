---
title: "Get accessReview"
description: "Read properties and relationships of the accessReview object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessReview

Namespace: microsoft.graph

Read properties and relationships of the [accessReview](../resources/accessreview.md) object.

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
GET /accessReviews/{accessReviewsId}
GET /accessReviews/{accessReviewsId}/instances/{accessReviewId}
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
If successful, this method returns a `200 OK` response code and [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accessreview"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1571

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReview",
    "id": "10b12c0e-2c0e-10b1-0e2c-b1100e2cb110",
    "displayName": "Display Name value",
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
    "status": "Status value",
    "createdBy": {
      "@odata.type": "microsoft.graph.userIdentity",
      "id": "Id value",
      "ipAddress": "Ip Address value",
      "userPrincipalName": "User Principal Name value"
    },
    "businessFlowTemplateId": "Business Flow Template Id value",
    "reviewerType": "Reviewer Type value",
    "description": "Description value",
    "settings": {
      "@odata.type": "microsoft.graph.accessReviewSettings",
      "mailNotificationsEnabled": true,
      "remindersEnabled": true,
      "justificationRequiredOnApproval": true,
      "recurrenceSettings": {
        "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings",
        "recurrenceType": "Recurrence Type value",
        "recurrenceEndType": "Recurrence End Type value",
        "durationInDays": 14,
        "recurrenceCount": 15
      },
      "autoReviewEnabled": true,
      "activityDurationInDays": 6,
      "autoReviewSettings": {
        "@odata.type": "microsoft.graph.autoReviewSettings",
        "notReviewedResult": "Not Reviewed Result value"
      },
      "autoApplyReviewResultsEnabled": true,
      "accessRecommendationsEnabled": true
    },
    "reviewedEntity": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

