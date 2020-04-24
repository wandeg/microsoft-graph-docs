---
title: "Update userConsentRequests"
description: "Update the properties of a userConsentRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userConsentRequests

Namespace: microsoft.graph

Update the properties of a userConsentRequests object.

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
PATCH /invitations/{invitationsId}/invitedUser/appConsentRequestsForApproval/{appConsentRequestId}/userConsentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [userConsentRequest](../resources/userconsentrequest.md) object.

The following table shows the properties that are required when you create the [userConsentRequest](../resources/userconsentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reason|String|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [userConsentRequest](../resources/userconsentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userconsentrequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/appConsentRequestsForApproval/{appConsentRequestId}/userConsentRequests
Content-Type: application/json
Content-length: 322

{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "reason": "Reason value",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "displayName": "Display Name value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "2088f674-f674-2088-74f6-882074f68820",
  "reason": "Reason value",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "Id value",
    "displayName": "Display Name value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  },
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
}
```

