---
title: "List roleAssignmentRequests"
description: "Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List roleAssignmentRequests

Namespace: microsoft.graph

Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.

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
GET ** Collection URI for microsoft.graph.governanceRoleAssignmentRequest not found
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

If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.governanceRoleAssignmentRequest not found
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governanceroleassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governanceRoleAssignmentRequest",
      "id": "f1870314-0314-f187-1403-87f1140387f1",
      "resourceId": "String",
      "roleDefinitionId": "String",
      "subjectId": "String",
      "linkedEligibleRoleAssignmentId": "String",
      "type": "String",
      "assignmentState": "String",
      "requestedDateTime": "String (timestamp)",
      "reason": "String",
      "status": {
        "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
      },
      "schedule": {
        "@odata.type": "microsoft.graph.governanceSchedule"
      }
    }
  ]
}
```

