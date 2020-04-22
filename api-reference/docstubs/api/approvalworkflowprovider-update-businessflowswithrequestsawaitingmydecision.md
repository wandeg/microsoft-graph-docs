---
title: "Update businessFlowsWithRequestsAwaitingMyDecision"
description: "Update the properties of a businessFlowsWithRequestsAwaitingMyDecision object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update businessFlowsWithRequestsAwaitingMyDecision

Namespace: microsoft.graph

Update the properties of a businessFlowsWithRequestsAwaitingMyDecision object.

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
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [businessFlow](../resources/businessflow.md) object.

The following table shows the properties that are required when you create the [businessFlow](../resources/businessflow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|deDuplicationId|String|**TODO: Add Description**|
|schemaId|String|**TODO: Add Description**|
|customData|String|**TODO: Add Description**|
|recordVersion|String|**TODO: Add Description**|
|policy|[governancePolicy](../resources/governancepolicy.md)|**TODO: Add Description**|
|policyTemplateId|String|**TODO: Add Description**|
|settings|[businessFlowSettings](../resources/businessflowsettings.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [businessFlow](../resources/businessflow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_businessflowswithrequestsawaitingmydecision"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision
Content-Type: application/json
Content-length: 1882

{
  "@odata.type": "#microsoft.graph.businessFlow",
  "displayName": "Display Name value",
  "description": "Description value",
  "deDuplicationId": "De Duplication Id value",
  "schemaId": "Schema Id value",
  "customData": "Custom Data value",
  "recordVersion": "Record Version value",
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
  "policyTemplateId": "Policy Template Id value",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.businessFlow",
  "id": "7a73fe53-fe53-7a73-53fe-737a53fe737a",
  "displayName": "Display Name value",
  "description": "Description value",
  "deDuplicationId": "De Duplication Id value",
  "schemaId": "Schema Id value",
  "customData": "Custom Data value",
  "recordVersion": "Record Version value",
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
  "policyTemplateId": "Policy Template Id value",
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

