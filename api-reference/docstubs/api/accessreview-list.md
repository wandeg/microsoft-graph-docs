---
title: "List accessReviews"
description: "Get a list of the accessReview objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessReviews

Namespace: microsoft.graph

Get a list of the [accessReview](../resources/accessreview.md) objects and their properties.

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
GET /accessReviews
GET /accessReviews/{accessReviewsId}/instances
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
If successful, this method returns a `200 OK` response code and a collection of [accessReview](../resources/accessreview.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accessreview"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviews
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessreview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReview",
      "id": "9b4ddbdb-dbdb-9b4d-dbdb-4d9bdbdb4d9b",
      "displayName": "Display Name value",
      "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
      "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
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
  ]
}
```

