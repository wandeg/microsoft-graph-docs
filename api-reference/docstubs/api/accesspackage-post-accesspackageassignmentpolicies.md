---
title: "Create accessPackageAssignmentPolicies"
description: "Create a new accessPackageAssignmentPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageAssignmentPolicies

Namespace: microsoft.graph

Create a new accessPackageAssignmentPolicies object.

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
POST /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|accessPackageId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|canExtend|Boolean|**TODO: Add Description**|
|durationInDays|Int32|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|requestorSettings|[requestorSettings](../resources/requestorsettings.md)|**TODO: Add Description**|
|requestApprovalSettings|[approvalSettings](../resources/approvalsettings.md)|**TODO: Add Description**|
|accessReviewSettings|[assignmentReviewSettings](../resources/assignmentreviewsettings.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies
Content-Type: application/json
Content-length: 1863

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
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
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "reviewers": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ]
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "8cb7d69e-d69e-8cb7-9ed6-b78c9ed6b78c",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "createdBy": "Created By value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
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
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "reviewers": [
      {
        "@odata.type": "microsoft.graph.singleUser"
      }
    ]
  }
}
```

