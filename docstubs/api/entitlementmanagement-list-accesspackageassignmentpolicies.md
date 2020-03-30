---
title: "List accessPackageAssignmentPolicies"
description: "Get the accessPackageAssignmentPolicies from the accessPackageAssignmentPolicies navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageAssignmentPolicies

Namespace: microsoft.graph

Get the accessPackageAssignmentPolicies from the accessPackageAssignmentPolicies navigation property.

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
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
      "id": "4564f3a3-f3a3-4564-a3f3-6445a3f36445",
      "accessPackageId": "Access Package Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "canExtend": true,
      "durationInDays": 14,
      "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
      "createdBy": "Created By value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:57:56.5934914+03:00",
      "requestorSettings": {
        "@odata.type": "microsoft.graph.requestorSettings",
        "scopeType": "Scope Type value",
        "acceptRequests": true,
        "allowedRequestors": [
          {
            "@odata.type": "microsoft.graph.singleUser",
            "isBackup": true,
            "id": "Id value"
          }
        ]
      },
      "requestApprovalSettings": {
        "@odata.type": "microsoft.graph.approvalSettings",
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": true,
        "isRequestorJustificationRequired": true,
        "approvalMode": "Approval Mode value",
        "approvalStages": [
          {
            "@odata.type": "microsoft.graph.approvalStage",
            "approvalStageTimeOutInDays": 10,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 7,
            "primaryApprovers": [
              {
                "@odata.type": "microsoft.graph.singleUser"
              }
            ],
            "escalationApprovers": [
              {
                "@odata.type": "microsoft.graph.singleUser"
              }
            ]
          }
        ]
      },
      "accessReviewSettings": {
        "@odata.type": "microsoft.graph.assignmentReviewSettings",
        "isEnabled": true,
        "recurrenceType": "Recurrence Type value",
        "reviewerType": "Reviewer Type value",
        "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
        "reviewers": [
          {
            "@odata.type": "microsoft.graph.singleUser"
          }
        ]
      }
    }
  ]
}
```

