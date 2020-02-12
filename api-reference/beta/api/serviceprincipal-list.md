---
title: "List servicePrincipals"
description: "Retrieve a list of servicePrincipal objects."
localization_priority: Normal
doc_type: apiPageType
ms.prod: "microsoft-identity-platform"
author: "davidmu1"
---

# List servicePrincipals

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve a list of servicePrincipal objects.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).


| Permission type | Permissions (from least to most privileged) |
|:--------------------|:---------------------------------------------------------|
| Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | Application.ReadWrite.All, Directory.Read.All |

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## Optional query parameters

This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. When resources are added using Microsoft Graph, they are indexed. This index is used for the `$count` and `$search` query parameters. There can be a slight delay between when a resource is added and when it is available in the index.

## Request headers

| Name | Description |
|:---- |:----------- |
| Authorization | Bearer {token}. Required. |
| ConsistencyLevel | The value is always `eventual`. This header is required when using the `$search` or `$count` query parameter. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.

## Examples

### Example 1: Get a list of service principal objects

#### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

### Example 2: Get a list of service principal objects including the count of returned objects

#### Request

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$count=true
```

#### Response

The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
ConsistencyLevel: eventual

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.count":100,
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
