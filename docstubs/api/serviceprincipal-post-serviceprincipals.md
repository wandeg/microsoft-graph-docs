---
title: "Create servicePrincipal"
description: "Create a new servicePrincipal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create servicePrincipal

Namespace: microsoft.graph

Create a new [servicePrincipal](../resources/serviceprincipal.md) object.

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
POST /servicePrincipals
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals
Content-type: application/json
Content-length: 3540

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "b4585226-5226-b458-2652-58b4265258b4",
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
  "appOwnerOrganizationId": "c34032d5-32d5-c340-d532-40c3d53240c3",
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
      "endDateTime": "2017-01-01T00:02:08.1909286+00:00",
      "keyId": "f43d4709-4709-f43d-0947-3df409473df4",
      "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
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
  "preferredTokenSigningKeyEndDateTime": "2017-01-01T00:02:50.2591452+00:00",
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
  "tokenEncryptionKeyId": "b155de0f-de0f-b155-0fde-55b10fde55b1"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3589

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
  "id": "1f5393ea-93ea-1f53-ea93-531fea93531f",
  "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "microsoft.graph.addIn",
      "id": "b4585226-5226-b458-2652-58b4265258b4",
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
  "appOwnerOrganizationId": "c34032d5-32d5-c340-d532-40c3d53240c3",
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
      "endDateTime": "2017-01-01T00:02:08.1909286+00:00",
      "keyId": "f43d4709-4709-f43d-0947-3df409473df4",
      "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
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
  "preferredTokenSigningKeyEndDateTime": "2017-01-01T00:02:50.2591452+00:00",
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
  "tokenEncryptionKeyId": "b155de0f-de0f-b155-0fde-55b10fde55b1"
}
```

