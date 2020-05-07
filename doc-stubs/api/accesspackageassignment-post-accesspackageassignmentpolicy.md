---
title: "Create accessPackageAssignmentPolicy"
description: "Create a new accessPackageAssignmentPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageAssignmentPolicy

Namespace: microsoft.graph

Create a new accessPackageAssignmentPolicy object.

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
POST ** Collection URI for microsoft.graph.accessPackageAssignmentPolicy not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.accessPackageAssignmentPolicy not found
Content-Type: application/json
Content-length: 597

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "accessPackageId": "String",
  "displayName": "String",
  "description": "String",
  "canExtend": "Boolean",
  "durationInDays": "Integer",
  "expirationDateTime": "String (timestamp)",
  "createdBy": "String",
  "modifiedBy": "String",
  "requestorSettings": {
    "@odata.type": "microsoft.graph.requestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.approvalSettings"
  },
  "accessReviewSettings": {
    "@odata.type": "microsoft.graph.assignmentReviewSettings"
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
  "id": "cb92e0a2-e0a2-cb92-a2e0-92cba2e092cb",
  "accessPackageId": "String",
  "displayName": "String",
  "description": "String",
  "canExtend": "Boolean",
  "durationInDays": "Integer",
  "expirationDateTime": "String (timestamp)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "requestorSettings": {
    "@odata.type": "microsoft.graph.requestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.approvalSettings"
  },
  "accessReviewSettings": {
    "@odata.type": "microsoft.graph.assignmentReviewSettings"
  }
}
```

