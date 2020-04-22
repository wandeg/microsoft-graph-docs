---
title: "List instances"
description: "Get the accessReviews from the instances navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List instances

Namespace: microsoft.graph

Get the accessReviews from the instances navigation property.

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
GET https://graph.microsoft.com/v1.0/accessReviews/{accessReviewsId}/instances
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "bd4245de-45de-bd42-de45-42bdde4542bd",
      "displayName": "Display Name value",
      "startDateTime": "2016-12-31T23:57:25.6506614+00:00",
      "endDateTime": "2016-12-31T23:59:23.0722644+00:00",
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

