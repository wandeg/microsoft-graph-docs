---
title: "List policyTemplates"
description: "Get the governancePolicyTemplates from the policyTemplates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List policyTemplates

Namespace: microsoft.graph

Get the governancePolicyTemplates from the policyTemplates navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [governancePolicyTemplate](../resources/governancepolicytemplate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governancepolicytemplate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governancepolicytemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1917

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governancePolicyTemplate",
      "id": "0a9b58f8-58f8-0a9b-f858-9b0af8589b0a",
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
  ]
}
```

