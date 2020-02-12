---
title: "List contacts"
description: "Get contacts in the user's mailbox."
localization_priority: Normal
author: "angelgolfer-ms"
ms.prod: "microsoft-identity-platform"
doc_type: apiPageType
---

# List contacts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get contacts in the user's mailbox.

There are two scenarios where an app can get contacts in another user's contact folder:

* If the app has application permissions, or,
* If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user. See [details and an example](/graph/outlook-get-shared-contacts-folders).


## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type | Permissions (from least to most privileged) |
|:-------------- |:------------------------------------------- |
| Delegated (work or school account) | Contacts.Read, Contacts.ReadWrite |
| Delegated (personal Microsoft account) | Contacts.Read, Contacts.ReadWrite |
| Application | Contacts.Read, Contacts.ReadWrite |

## HTTP request

To get all the contacts in a user's mailbox:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

To get contacts in a specific folder in the user's mailbox:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## Optional query parameters

You can use the `$filter` query parameter to filter contacts based on their email addresses:

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection. That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.

You can also use the `$count` and `$search` query parameters to limit the response. When resources are added using Microsoft Graph, they are indexed. This index is used for the `$count` and `$search` query parameters. There can be a slight delay between when a resource is added and when it is available in the index.

For general information on the `$filter`, `$count`, and `$search` query parameter, see [OData query parameters](/graph/query-parameters).

## Request headers

| Header | Value |
|:------ |:--------|
| Authorization | Bearer {token}. Required. |
| ConsistencyLevel | Value is always `eventual`. This header is required when using the `$search` or `$count` query parameter. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.

## Examples

### Example 1: Get contacts in the user's mailbox

#### Request

The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```
# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

Here is an example of the response. 
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('id-value')/contacts(displayName,emailAddresses)",
  "value":[
    {
      "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
      "id":"AAMkADh6v5AAAvgTCFAAA=",
      "displayName":"Elvis Blank",
      "emailAddresses":[
        {
          "type":"personal",
          "name":"Elvis Blank",
          "address":"elvisb@relecloud.onmicrosoft.com"
        },
        {
          "type":"other",
          "otherLabel":"Volunteer work",
          "name":"Elvis Blank",
          "address":"elvisb@fabrikam.onmicrosoft.com"
        }
      ]
    },
    {
      "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
      "id":"AAMkADh6v5AAAvgTCEAAA=",
      "displayName":"Pavel Bansky",
      "emailAddresses":[
        {
          "type":"personal",
          "name":"Pavel Bansky",
          "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
          "type":"other",
          "otherLabel":"Volunteer work",
          "name":"Pavel Bansky",
          "address":"pavelb@fabrikam.onmicrosoft.com"
        }
      ]
    }
  ]
}
```

### Example 2: Get contacts in the user's mailbox including the count of returned objects

#### Request

The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts and the nu,ber of objects returned.

<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts?$count=true$select=displayName,emailAddresses
```

#### Response

Here is an example of the response. 
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
ConsistencyLevel: eventual

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('id-value')/contacts(displayName,emailAddresses)",
  "@odata.count":2,
  "value":[
    {
      "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
      "id":"AAMkADh6v5AAAvgTCFAAA=",
      "displayName":"Elvis Blank",
      "emailAddresses":[
        {
          "type":"personal",
          "name":"Elvis Blank",
          "address":"elvisb@relecloud.onmicrosoft.com"
        },
        {
          "type":"other",
          "otherLabel":"Volunteer work",
          "name":"Elvis Blank",
          "address":"elvisb@fabrikam.onmicrosoft.com"
        }
      ]
    },
    {
      "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
      "id":"AAMkADh6v5AAAvgTCEAAA=",
      "displayName":"Pavel Bansky",
      "emailAddresses":[
        {
          "type":"personal",
          "name":"Pavel Bansky",
          "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
          "type":"other",
          "otherLabel":"Volunteer work",
          "name":"Pavel Bansky",
          "address":"pavelb@fabrikam.onmicrosoft.com"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
