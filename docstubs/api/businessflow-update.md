---
title: "Update businessFlow"
description: "Update the properties of a businessFlow object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update businessFlow

Namespace: microsoft.graph

Update the properties of a [businessFlow](../resources/businessflow.md) object.

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
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}
PATCH /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision/{businessFlowId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [businessFlow](../resources/businessflow.md) object.

The following table shows the properties that are required when you create the [businessFlow](../resources/businessflow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|deDuplicationId|String||
|schemaId|String||
|customData|String||
|recordVersion|String||
|policy|[governancePolicy](../resources/governancepolicy.md)||
|policyTemplateId|String||
|settings|[businessFlowSettings](../resources/businessflowsettings.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [businessFlow](../resources/businessflow.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_businessflow"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1931

{
  "@odata.type": "#microsoft.graph.businessFlow",
  "id": "4b7a573e-573e-4b7a-3e57-7a4b3e577a4b",
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

