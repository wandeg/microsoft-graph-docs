---
title: "Get businessFlow"
description: "Read the properties and relationships of a businessFlow object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get businessFlow

Namespace: microsoft.graph

Read the properties and relationships of a [businessFlow](../resources/businessflow.md) object.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision/{businessFlowId}
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
If successful, this method returns a `200 OK` response code and a [businessFlow](../resources/businessflow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_businessflow"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlows/{businessFlowId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.businessFlow",
    "id": "c6a5b2c1-b2c1-c6a5-c1b2-a5c6c1b2a5c6",
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
}
```

