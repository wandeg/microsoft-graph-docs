---
title: "Get accessPackageAssignmentPolicy"
description: "Read the properties and relationships of an accessPackageAssignmentPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get accessPackageAssignmentPolicy

Namespace: microsoft.graph

Read the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

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
GET /accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentPolicies/{accessPackageAssignmentPoliciesId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

