---
title: "List intendedPolicies"
description: "Get the managedAppPolicies from the intendedPolicies navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List intendedPolicies

Namespace: microsoft.graph

Get the managedAppPolicies from the intendedPolicies navigation property.

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
GET /invitations/{invitationsId}/invitedUser/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
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
If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/managedapppolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managedapppolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedapppolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "id": "af6c0cd8-0cd8-af6c-d80c-6cafd80c6caf",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
      "version": "Version value"
    }
  ]
}
```

