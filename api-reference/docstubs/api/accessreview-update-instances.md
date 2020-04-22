---
title: "Update instances"
description: "Update the properties of an instances object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update instances

Namespace: microsoft.graph

Update the properties of an instances object.

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
PATCH /accessReviews/{accessReviewsId}/instances
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [accessReview](../resources/accessreview.md) object.

The following table shows the properties that are required when you create the [accessReview](../resources/accessreview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|businessFlowTemplateId|String|**TODO: Add Description**|
|reviewerType|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)|**TODO: Add Description**|
|reviewedEntity|[identity](../resources/identity.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_instances"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}/instances
Content-Type: application/json
Content-length: 1425

{
  "@odata.type": "#microsoft.graph.accessReview",
  "displayName": "Display Name value",
  "startDateTime": "2017-01-01T00:00:43.6519742+00:00",
  "endDateTime": "2017-01-01T00:02:18.2306619+00:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "dafde566-e566-dafd-66e5-fdda66e5fdda",
  "displayName": "Display Name value",
  "startDateTime": "2017-01-01T00:00:43.6519742+00:00",
  "endDateTime": "2017-01-01T00:02:18.2306619+00:00",
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

