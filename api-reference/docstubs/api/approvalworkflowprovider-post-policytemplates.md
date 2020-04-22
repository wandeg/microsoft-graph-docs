---
title: "Create policyTemplates"
description: "Create a new policyTemplates object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create policyTemplates

Namespace: microsoft.graph

Create a new policyTemplates object.

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
POST /approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.

The following table shows the properties that are required when you create the [governancePolicyTemplate](../resources/governancepolicytemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|policy|[governancePolicy](../resources/governancepolicy.md)|**TODO: Add Description**|
|settings|[businessFlowSettings](../resources/businessflowsettings.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_governancepolicytemplate_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates
Content-Type: application/json
Content-length: 1639

{
  "@odata.type": "#microsoft.graph.governancePolicyTemplate",
  "displayName": "Display Name value",
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
          "id": "Id value",
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
    "@odata.type": "microsoft.graph.businessFlowSettings",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governancepolicytemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.governancePolicyTemplate",
  "id": "1610d5d5-d5d5-1610-d5d5-1016d5d51016",
  "displayName": "Display Name value",
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
          "id": "Id value",
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
    "@odata.type": "microsoft.graph.businessFlowSettings",
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

