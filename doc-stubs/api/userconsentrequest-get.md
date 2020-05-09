---
title: "Get userConsentRequest"
description: "Read the properties and relationships of a userConsentRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get userConsentRequest

Namespace: microsoft.graph

Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.

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
GET /me/appConsentRequestsForApproval/{appConsentRequestId}/userConsentRequests/{userConsentRequestId}
GET /users/{usersId}/appConsentRequestsForApproval/{appConsentRequestId}/userConsentRequests/{userConsentRequestId}
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

If successful, this method returns a `200 OK` response code and a [userConsentRequest](../resources/userconsentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/appConsentRequestsForApproval/{appConsentRequestId}/userConsentRequests/{userConsentRequestId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.userConsentRequest",
    "id": "11c912f0-12f0-11c9-f012-c911f012c911",
    "reason": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.userIdentity"
    },
    "createdDateTime": "String (timestamp)"
  }
}
```

