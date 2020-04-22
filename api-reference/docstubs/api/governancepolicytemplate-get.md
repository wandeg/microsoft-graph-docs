---
title: "Get governancePolicyTemplate"
description: "Read properties and relationships of a governancePolicyTemplate object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get governancePolicyTemplate

Namespace: microsoft.graph

Read properties and relationships of a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates/{governancePolicyTemplateId}
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
If successful, this method returns a `200 OK` response code and a [governancePolicyTemplate](../resources/governancepolicytemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_governancepolicytemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates/{governancePolicyTemplateId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governancePolicyTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

