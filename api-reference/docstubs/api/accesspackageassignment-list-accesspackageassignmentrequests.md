---
title: "List accessPackageAssignmentRequests"
description: "Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageAssignmentRequests

Namespace: microsoft.graph

Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.

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
GET /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentRequests
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
      "id": "a571c5ac-c5ac-a571-acc5-71a5acc571a5",
      "requestType": "Request Type value",
      "requestState": "Request State value",
      "requestStatus": "Request Status value",
      "isValidationOnly": true,
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "completedDate": "2016-12-31T23:59:42.8740055+03:00",
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
      "justification": "Justification value"
    }
  ]
}
```

