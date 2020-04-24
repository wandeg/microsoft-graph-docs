---
title: "Create accessPackageAssignments"
description: "Create a new accessPackageAssignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageAssignments

Namespace: microsoft.graph

Create a new accessPackageAssignments object.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageAssignment](../resources/accesspackageassignment.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignment](../resources/accesspackageassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|catalogId|String|**TODO: Add Description**|
|accessPackageId|String|**TODO: Add Description**|
|assignmentPolicyId|String|**TODO: Add Description**|
|targetId|String|**TODO: Add Description**|
|assignmentStatus|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|isExtended|Boolean|**TODO: Add Description**|
|expiredDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageAssignment](../resources/accesspackageassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignment_from_accesspackageassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
Content-Type: application/json
Content-length: 419

{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "catalogId": "Catalog Id value",
  "accessPackageId": "Access Package Id value",
  "assignmentPolicyId": "Assignment Policy Id value",
  "targetId": "Target Id value",
  "assignmentStatus": "Assignment Status value",
  "assignmentState": "Assignment State value",
  "isExtended": true,
  "expiredDateTime": "2016-12-31T23:57:03.8636442+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "6f11a7e3-a7e3-6f11-e3a7-116fe3a7116f",
  "catalogId": "Catalog Id value",
  "accessPackageId": "Access Package Id value",
  "assignmentPolicyId": "Assignment Policy Id value",
  "targetId": "Target Id value",
  "assignmentStatus": "Assignment Status value",
  "assignmentState": "Assignment State value",
  "isExtended": true,
  "expiredDateTime": "2016-12-31T23:57:03.8636442+03:00"
}
```

