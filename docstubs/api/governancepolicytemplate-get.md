---
title: "Get governancePolicyTemplate"
description: "Read properties and relationships of the governancePolicyTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governancePolicyTemplate

Namespace: microsoft.graph

Read properties and relationships of the [governancePolicyTemplate](../resources/governancepolicytemplate.md) object.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates/{governancePolicyTemplateId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [governancePolicyTemplate](../resources/governancepolicytemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governancepolicytemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/policyTemplates/{governancePolicyTemplateId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governancePolicyTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1805

{
  "value": {
    "@odata.type": "#microsoft.graph.governancePolicyTemplate",
    "id": "f78fdffd-dffd-f78f-fddf-8ff7fddf8ff7",
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

