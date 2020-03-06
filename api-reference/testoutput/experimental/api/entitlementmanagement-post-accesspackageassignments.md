---
title: "Add accessPackageAssignments"
description: "Add accessPackageAssignments by posting to the accessPackageAssignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageAssignments

Namespace: microsoft.graph

Add accessPackageAssignments by posting to the accessPackageAssignments collection.

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
POST /identityGovernance/entitlementManagement/accessPackageAssignments/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignment](../resources/accesspackageassignment.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignment](../resources/accesspackageassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|catalogId|String||
|accessPackageId|String||
|assignmentPolicyId|String||
|targetId|String||
|assignmentStatus|String||
|assignmentState|String||
|isExtended|Boolean||
|expiredDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageAssignment](../resources/accesspackageassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignment_from_accesspackageassignments"
}
-->
``` http
POST https://graph.microsoft.com/localtest/identityGovernance/entitlementManagement/accessPackageAssignments
Content-type: application/json
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
  "expiredDateTime": "2017-01-01T00:03:03.9221806+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 468

{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "e4383339-3339-e438-3933-38e4393338e4",
  "catalogId": "Catalog Id value",
  "accessPackageId": "Access Package Id value",
  "assignmentPolicyId": "Assignment Policy Id value",
  "targetId": "Target Id value",
  "assignmentStatus": "Assignment Status value",
  "assignmentState": "Assignment State value",
  "isExtended": true,
  "expiredDateTime": "2017-01-01T00:03:03.9221806+03:00"
}
```

