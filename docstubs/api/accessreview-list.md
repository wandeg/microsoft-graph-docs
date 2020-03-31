---
title: "List accessReviews"
description: "List properties and relationships of the accessReview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessReviews

Namespace: microsoft.graph

List properties and relationships of the [accessReview](../resources/accessreview.md) objects.

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
GET /accessReviews
GET /accessReviews/{accessReviewsId}/instances
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
If successful, this method returns a `200 OK` response code and a collection of [accessReview](../resources/accessreview.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accessreview"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessReviews
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessreview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReview",
      "id": "65d727dc-27dc-65d7-dc27-d765dc27d765",
      "displayName": "Display Name value",
      "startDateTime": "2017-01-01T00:03:09.5259332+03:00",
      "endDateTime": "2016-12-31T23:57:04.2596185+03:00",
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

