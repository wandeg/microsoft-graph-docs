---
title: "Update accessReview"
description: "Update the properties of a accessReview object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessReview

Namespace: microsoft.graph

Update the properties of a [accessReview](../resources/accessreview.md) object.

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
PATCH /accessReviews/{accessReviewsId}
PATCH /accessReviews/{accessReviewsId}/instances/{accessReviewId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [accessReview](../resources/accessreview.md) object.

The following table shows the properties that are required when you create the [accessReview](../resources/accessreview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|status|String||
|createdBy|[userIdentity](../resources/useridentity.md)||
|businessFlowTemplateId|String||
|reviewerType|String||
|description|String||
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)||
|reviewedEntity|[identity](../resources/identity.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accessreview"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}
Content-type: application/json
Content-length: 1423

{
  "@odata.type": "#microsoft.graph.accessReview",
  "displayName": "Display Name value",
  "startDateTime": "2016-12-31T23:57:40.5444496+00:00",
  "endDateTime": "2016-12-31T23:58:47.51829+00:00",
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
Content-Length: 1472

{
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "3ead990d-990d-3ead-0d99-ad3e0d99ad3e",
  "displayName": "Display Name value",
  "startDateTime": "2016-12-31T23:57:40.5444496+00:00",
  "endDateTime": "2016-12-31T23:58:47.51829+00:00",
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
```

