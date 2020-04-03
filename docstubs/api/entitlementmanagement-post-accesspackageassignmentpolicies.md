---
title: "Add accessPackageAssignmentPolicies"
description: "Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageAssignmentPolicies

Namespace: microsoft.graph

Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|accessPackageId|String||
|displayName|String||
|description|String||
|canExtend|Boolean||
|durationInDays|Int32||
|expirationDateTime|DateTimeOffset||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||
|requestorSettings|[requestorSettings](../resources/requestorsettings.md)||
|requestApprovalSettings|[approvalSettings](../resources/approvalsettings.md)||
|accessReviewSettings|[assignmentReviewSettings](../resources/assignmentreviewsettings.md)||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json
Content-length: 1864

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value",
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
    "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
    "reviewers": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ]
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2032

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "e3e85c70-5c70-e3e8-705c-e8e3705ce8e3",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00",
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
    "startDateTime": "2016-12-31T23:59:00.3105042+00:00",
    "reviewers": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ]
  }
}
```

