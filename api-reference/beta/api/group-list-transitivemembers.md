---
title: "List group transitive members"
description: "Get a list of the group's members. A group can have users, contacts, devices, service principals and other groups as members. This operation is transitive and will also return a flat list of all nested members."
localization_priority: Normal
author: "dkershaw10"
ms.prod: "groups"
doc_type: apiPageType
---

# List group transitive members

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the group's members. A group can have users, contacts, devices, service principals and other groups as members. This operation is transitive and will also return a flat list of all nested members.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type | Permissions (from least to most privileged) |
|:--------------- |:------------------------------------------- |
| Delegated (work or school account) | Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All    |
| Delegated (personal Microsoft account) | Not supported. |
| Application | Directory.Read.All, User.Read.All |

> Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## Optional query parameters

This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response. When resources are added using Microsoft Graph, they are indexed. This index is used for the `$count` and `$search` query parameters. There can be a slight delay between when a resource is added and when it is available in the index.

## Request headers

| Name | Description |
|:---- |:----------- |
| Authorization  | Bearer {token}. Required. |
| ConsistencyLevel | Value is always `eventual`. This header is required when using the `$count` and `$search` query parameters. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.

## Examples

### Example 1: Get a list of the group's members

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### Example 2: Get a transitive list of groups with a specific display name including the count of returned objects 

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$/Microsoft.Graph.Group?$filter=startswith(displayName,'Contoso')&$count=true&$select=displayName, id 
```

#### Response

The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
ConsistencyLevel: eventual

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":3,
  "value":[
    {
      "displayName":"Contoso 1",
      "id":"id-value"
    },
    {
      "displayName":"Contoso 2",
      "id":"id-value"
    },
    {
      "displayName":"Contoso 3",
      "id":"id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
