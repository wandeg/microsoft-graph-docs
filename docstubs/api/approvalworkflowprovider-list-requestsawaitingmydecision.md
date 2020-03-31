---
title: "List requestsAwaitingMyDecision"
description: "Get the requests from the requestsAwaitingMyDecision navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List requestsAwaitingMyDecision

Namespace: microsoft.graph

Get the requests from the requestsAwaitingMyDecision navigation property.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/requestsAwaitingMyDecision
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
If successful, this method returns a `200 OK` response code and a collection of [request](../resources/request.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_request"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/requestsAwaitingMyDecision
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.request)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2565

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.request",
      "id": "a299295a-295a-a299-5a29-99a25a2999a2",
      "displayName": "Display Name value",
      "description": "Description value",
      "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
      "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
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
  ]
}
```

