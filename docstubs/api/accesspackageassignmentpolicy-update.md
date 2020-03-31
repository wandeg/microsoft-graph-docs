---
title: "Update accessPackageAssignmentPolicy"
description: "Update the properties of a accessPackageAssignmentPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update accessPackageAssignmentPolicy

Namespace: microsoft.graph

Update the properties of a [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

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
PATCH /accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
PATCH /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentPolicy
PATCH /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
PATCH /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentPolicy
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
Content-type: application/json
Content-length: 1864

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
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
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2032

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "e7b87e5e-7e5e-e7b8-5e7e-b8e75e7eb8e7",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:03:28.4967331+03:00",
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
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
    "reviewers": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ]
  }
}
```

