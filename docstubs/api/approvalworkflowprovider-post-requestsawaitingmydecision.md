---
title: "Add requestsAwaitingMyDecision"
description: "Add requestsAwaitingMyDecision by posting to the requestsAwaitingMyDecision collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add requestsAwaitingMyDecision

Namespace: microsoft.graph

Add requestsAwaitingMyDecision by posting to the requestsAwaitingMyDecision collection.

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
POST /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requestsAwaitingMyDecision/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [request](../resources/request.md) object.

The following table shows the properties that are required when you create the [request](../resources/request.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|status|String||
|businessFlowId|String||
|createdBy|[userIdentity](../resources/useridentity.md)||
|deDuplicationId|String||
|schemaId|String||
|customData|String||
|recordVersion|String||
|policyTemplateId|String||
|policy|[governancePolicy](../resources/governancepolicy.md)||
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)||



## Response
If successful, this method returns a `201 Created` response code and a [request](../resources/request.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_request_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/requestsAwaitingMyDecision
Content-type: application/json
Content-length: 2227

{
  "@odata.type": "#microsoft.graph.request",
  "displayName": "Display Name value",
  "description": "Description value",
  "startDateTime": "2016-12-31T23:58:03.4514069+03:00",
  "endDateTime": "2017-01-01T00:00:11.5602866+03:00",
  "status": "Status value",
  "businessFlowId": "Business Flow Id value",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "deDuplicationId": "De Duplication Id value",
  "schemaId": "Schema Id value",
  "customData": "Custom Data value",
  "recordVersion": "Record Version value",
  "policyTemplateId": "Policy Template Id value",
  "policy": {
    "@odata.type": "microsoft.graph.governancePolicy",
    "decisionMakerCriteria": [
      {
        "@odata.type": "microsoft.graph.groupMembershipGovernanceCriteria",
        "groupId": "Group Id value"
      }
    ],
    "notificationPolicy": {
      "@odata.type": "microsoft.graph.governanceNotificationPolicy",
      "notificationTemplates": [
        {
          "@odata.type": "microsoft.graph.governanceNotificationTemplate",
          "type": "Type value",
          "source": "Source value",
          "version": "Version value",
          "culture": "Culture value"
        }
      ],
      "enabledTemplateTypes": [
        "Enabled Template Types value"
      ]
    }
  },
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
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.request"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2276

{
  "@odata.type": "#microsoft.graph.request",
  "id": "d0b37889-7889-d0b3-8978-b3d08978b3d0",
  "displayName": "Display Name value",
  "description": "Description value",
  "startDateTime": "2016-12-31T23:58:03.4514069+03:00",
  "endDateTime": "2017-01-01T00:00:11.5602866+03:00",
  "status": "Status value",
  "businessFlowId": "Business Flow Id value",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "deDuplicationId": "De Duplication Id value",
  "schemaId": "Schema Id value",
  "customData": "Custom Data value",
  "recordVersion": "Record Version value",
  "policyTemplateId": "Policy Template Id value",
  "policy": {
    "@odata.type": "microsoft.graph.governancePolicy",
    "decisionMakerCriteria": [
      {
        "@odata.type": "microsoft.graph.groupMembershipGovernanceCriteria",
        "groupId": "Group Id value"
      }
    ],
    "notificationPolicy": {
      "@odata.type": "microsoft.graph.governanceNotificationPolicy",
      "notificationTemplates": [
        {
          "@odata.type": "microsoft.graph.governanceNotificationTemplate",
          "type": "Type value",
          "source": "Source value",
          "version": "Version value",
          "culture": "Culture value"
        }
      ],
      "enabledTemplateTypes": [
        "Enabled Template Types value"
      ]
    }
  },
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
  }
}
```

