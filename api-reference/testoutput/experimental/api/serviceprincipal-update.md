---
title: "Update servicePrincipal"
description: "Update the properties of a servicePrincipal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update servicePrincipal

Namespace: microsoft.graph

Update the properties of a [servicePrincipal](../resources/serviceprincipal.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /servicePrincipals/{servicePrincipalsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [servicePrincipal](../resources/serviceprincipal.md) object.

The following table shows the properties that are required when you create the [servicePrincipal](../resources/serviceprincipal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|accountEnabled|Boolean||
|addIns|[addIn](../resources/addin.md) collection||
|appDisplayName|String||
|appId|String||
|applicationTemplateId|String||
|appOwnerOrganizationId|Guid||
|appRoleAssignmentRequired|Boolean||
|appRoles|[appRole](../resources/approle.md) collection||
|displayName|String||
|homepage|String||
|keyCredentials|[keyCredential](../resources/keycredential.md) collection||
|info|[informationalUrl](../resources/informationalurl.md)||
|logoutUrl|String||
|notificationEmailAddresses|String collection||
|publishedPermissionScopes|[permissionScope](../resources/permissionscope.md) collection||
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection||
|preferredTokenSigningKeyThumbprint|String||
|publisherName|String||
|replyUrls|String collection||
|samlMetadataUrl|String||
|servicePrincipalNames|String collection||
|tags|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/servicePrincipals/{servicePrincipalsId}
Content-type: application/json
Content-length: 2916

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "e9c8bcc9-bcc9-e9c8-c9bc-c8e9c9bcc8e9",
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
  "appOwnerOrganizationId": "6c64b8b7-b8b7-6c64-b7b8-646cb7b8646c",
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
      "endDateTime": "2017-01-01T00:02:18.392989+03:00",
      "keyId": "5c0881d6-81d6-5c08-d681-085cd681085c",
      "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2965

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "id": "0cf3ca8d-ca8d-0cf3-8dca-f30c8dcaf30c",
  "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "e9c8bcc9-bcc9-e9c8-c9bc-c8e9c9bcc8e9",
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
  "appOwnerOrganizationId": "6c64b8b7-b8b7-6c64-b7b8-646cb7b8646c",
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
      "endDateTime": "2017-01-01T00:02:18.392989+03:00",
      "keyId": "5c0881d6-81d6-5c08-d681-085cd681085c",
      "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
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
```

