---
title: "List servicePrincipals"
description: "Get a list of the servicePrincipal objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List servicePrincipals

Namespace: microsoft.graph

Get a list of the [servicePrincipal](../resources/serviceprincipal.md) objects and their properties.

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
GET /servicePrincipals
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
If successful, this method returns a `200 OK` response code and a collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.serviceprincipal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "71d9d353-d353-71d9-53d3-d97153d3d971",
      "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
      "accountEnabled": true,
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn",
          "id": "081ab855-b855-081a-55b8-1a0855b81a08",
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
      "alternativeNames": [
        "Alternative Names value"
      ],
      "appDisplayName": "App Display Name value",
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appOwnerOrganizationId": "a9ffb1a2-b1a2-a9ff-a2b1-ffa9a2b1ffa9",
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
      "errorUrl": "https://example.com/errorUrl/",
      "homepage": "Homepage value",
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl",
        "logoUrl": "https://example.com/logoUrl/",
        "marketingUrl": "https://example.com/marketingUrl/",
        "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
        "supportUrl": "https://example.com/supportUrl/",
        "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
      },
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential",
          "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
          "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
          "keyId": "3378f387-f387-3378-87f3-783387f37833",
          "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
          "usage": "Usage value",
          "key": "a2V5"
        }
      ],
      "loginUrl": "https://example.com/loginUrl/",
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
      "preferredTokenSigningKeyEndDateTime": "2017-01-01T00:01:57.4251884+03:00",
      "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
      "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
      "publisherName": "Publisher Name value",
      "replyUrls": [
        "Reply Urls value"
      ],
      "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
      "samlSingleSignOnSettings": {
        "@odata.type": "microsoft.graph.samlSingleSignOnSettings",
        "relayState": "Relay State value"
      },
      "servicePrincipalNames": [
        "Service Principal Names value"
      ],
      "servicePrincipalType": "Service Principal Type value",
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "ca3fb1e4-b1e4-ca3f-e4b1-3fcae4b13fca"
    }
  ]
}
```

