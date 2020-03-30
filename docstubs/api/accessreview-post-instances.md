---
title: "Add instances"
description: "Add instances by posting to the instances collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add instances

Namespace: microsoft.graph

Add instances by posting to the instances collection.

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
POST /accessReviews/{accessReviewsId}/instances/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accessreview_from_accessreviews"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/instances
Content-type: application/json
Content-length: 1425

{
  "@odata.type": "#microsoft.graph.accessReview",
  "displayName": "Display Name value",
  "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
  "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.accessreview"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1474

{
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "fa5ed667-d667-fa5e-67d6-5efa67d65efa",
  "displayName": "Display Name value",
  "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
  "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
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

