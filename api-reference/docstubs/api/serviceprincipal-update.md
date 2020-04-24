---
title: "Update servicePrincipal"
description: "Update the properties of a servicePrincipal object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update servicePrincipal

Namespace: microsoft.graph

Update the properties of a [servicePrincipal](../resources/serviceprincipal.md) object.

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
PATCH /servicePrincipals/{servicePrincipalsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [servicePrincipal](../resources/serviceprincipal.md) object.

The following table shows the properties that are required when you create the [servicePrincipal](../resources/serviceprincipal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|accountEnabled|Boolean|**TODO: Add Description**|
|addIns|[addIn](../resources/addin.md) collection|**TODO: Add Description**|
|alternativeNames|String collection|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|applicationTemplateId|String|**TODO: Add Description**|
|appOwnerOrganizationId|Guid|**TODO: Add Description**|
|appRoleAssignmentRequired|Boolean|**TODO: Add Description**|
|appRoles|[appRole](../resources/approle.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|errorUrl|String|**TODO: Add Description**|
|homepage|String|**TODO: Add Description**|
|info|[informationalUrl](../resources/informationalurl.md)|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|loginUrl|String|**TODO: Add Description**|
|logoutUrl|String|**TODO: Add Description**|
|notificationEmailAddresses|String collection|**TODO: Add Description**|
|publishedPermissionScopes|[permissionScope](../resources/permissionscope.md) collection|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description**|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|**TODO: Add Description**|
|preferredTokenSigningKeyThumbprint|String|**TODO: Add Description**|
|preferredSingleSignOnMode|String|**TODO: Add Description**|
|publisherName|String|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|
|samlMetadataUrl|String|**TODO: Add Description**|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|**TODO: Add Description**|
|servicePrincipalNames|String collection|**TODO: Add Description**|
|servicePrincipalType|String|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}
Content-Type: application/json
Content-length: 3540

{
  "@odata.type": "#microsoft.graph.servicePrincipal",
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
```

