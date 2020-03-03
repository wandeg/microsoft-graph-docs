---
title: "Get servicePrincipal"
description: "Read properties and relationships of the servicePrincipal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get servicePrincipal

Namespace: microsoft.graph

Read properties and relationships of the [servicePrincipal](../resources/serviceprincipal.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /servicePrincipals/{servicePrincipalsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/localtest/servicePrincipals/{servicePrincipalsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3161

{
  "value": {
    "@odata.type": "#microsoft.graph.servicePrincipal",
    "id": "da5b47bc-47bc-da5b-bc47-5bdabc475bda",
    "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
    "accountEnabled": true,
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "id": "cdc6f9dc-f9dc-cdc6-dcf9-c6cddcf9c6cd",
        "type": "Type value",
        "properties": [
          {
            "@odata.type": "microsoft.graph.keyValue",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      }
    ],
    "appDisplayName": "App Display Name value",
    "appId": "App Id value",
    "applicationTemplateId": "Application Template Id value",
    "appOwnerOrganizationId": "9f15957f-957f-9f15-7f95-159f7f95159f",
    "appRoleAssignmentRequired": true,
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole",
        "allowedMemberTypes": [
          "Allowed Member Types value"
        ],
        "description": "Description value",
        "displayName": "Display Name value",
        "isEnabled": true,
        "origin": "Origin value"
      }
    ],
    "displayName": "Display Name value",
    "homepage": "Homepage value",
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential",
        "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
        "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
        "keyId": "6b92b784-b784-6b92-84b7-926b84b7926b",
        "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
        "usage": "Usage value",
        "key": "a2V5"
      }
    ],
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl",
      "logoUrl": "https://example.com/logoUrl/",
      "marketingUrl": "https://example.com/marketingUrl/",
      "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
      "supportUrl": "https://example.com/supportUrl/",
      "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
    },
    "logoutUrl": "https://example.com/logoutUrl/",
    "notificationEmailAddresses": [
      "Notification Email Addresses value"
    ],
    "publishedPermissionScopes": [
      {
        "@odata.type": "microsoft.graph.permissionScope",
        "adminConsentDescription": "Admin Consent Description value",
        "adminConsentDisplayName": "Admin Consent Display Name value",
        "userConsentDescription": "User Consent Description value",
        "userConsentDisplayName": "User Consent Display Name value"
      }
    ],
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential",
        "secretText": "Secret Text value",
        "hint": "Hint value"
      }
    ],
    "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
    "publisherName": "Publisher Name value",
    "replyUrls": [
      "Reply Urls value"
    ],
    "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
    "servicePrincipalNames": [
      "Service Principal Names value"
    ],
    "tags": [
      "Tags value"
    ]
  }
}
```

