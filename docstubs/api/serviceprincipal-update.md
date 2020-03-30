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
|Name|Description|
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
|alternativeNames|String collection||
|appDisplayName|String||
|appId|String||
|applicationTemplateId|String||
|appOwnerOrganizationId|Guid||
|appRoleAssignmentRequired|Boolean||
|appRoles|[appRole](../resources/approle.md) collection||
|displayName|String||
|errorUrl|String||
|homepage|String||
|info|[informationalUrl](../resources/informationalurl.md)||
|keyCredentials|[keyCredential](../resources/keycredential.md) collection||
|loginUrl|String||
|logoutUrl|String||
|notificationEmailAddresses|String collection||
|publishedPermissionScopes|[permissionScope](../resources/permissionscope.md) collection||
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection||
|preferredTokenSigningKeyEndDateTime|DateTimeOffset||
|preferredTokenSigningKeyThumbprint|String||
|preferredSingleSignOnMode|String||
|publisherName|String||
|replyUrls|String collection||
|samlMetadataUrl|String||
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)||
|servicePrincipalNames|String collection||
|servicePrincipalType|String||
|signInAudience|String||
|tags|String collection||
|tokenEncryptionKeyId|Guid||



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
PATCH https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}
Content-type: application/json
Content-length: 3540

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "698f6327-6327-698f-2763-8f6927638f69",
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
  "appOwnerOrganizationId": "5423eb42-eb42-5423-42eb-235442eb2354",
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
      "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
      "keyId": "8bcecebf-cebf-8bce-bfce-ce8bbfcece8b",
      "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
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
  "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:58.1401917+00:00",
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
  "tokenEncryptionKeyId": "373f31b3-31b3-373f-b331-3f37b3313f37"
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
Content-Length: 3589

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "id": "6f4bbe04-be04-6f4b-04be-4b6f04be4b6f",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "698f6327-6327-698f-2763-8f6927638f69",
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
  "appOwnerOrganizationId": "5423eb42-eb42-5423-42eb-235442eb2354",
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
      "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
      "keyId": "8bcecebf-cebf-8bce-bfce-ce8bbfcece8b",
      "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
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
  "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:58.1401917+00:00",
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
  "tokenEncryptionKeyId": "373f31b3-31b3-373f-b331-3f37b3313f37"
}
```

