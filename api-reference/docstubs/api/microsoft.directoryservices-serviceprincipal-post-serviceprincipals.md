---
title: "Create servicePrincipal"
description: "Create a new servicePrincipal object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create servicePrincipal

Namespace: Microsoft.DirectoryServices

Create a new [servicePrincipal](../resources/microsoft.directoryservices-serviceprincipal.md) object.

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
POST /servicePrincipals
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [servicePrincipal](../resources/microsoft.directoryservices-serviceprincipal.md) object.

The following table shows the properties that are required when you create the [servicePrincipal](../resources/microsoft.directoryservices-serviceprincipal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|accountEnabled|Boolean|**TODO: Add Description**|
|addIns|[addIn](../resources/microsoft.directoryservices-addin.md) collection|**TODO: Add Description**|
|alternativeNames|String collection|**TODO: Add Description**|
|api|[apiServicePrincipal](../resources/microsoft.directoryservices-apiserviceprincipal.md)|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|applicationTemplateId|String|**TODO: Add Description**|
|appOwnerOrganizationId|Guid|**TODO: Add Description**|
|appRoleAssignmentRequired|Boolean|**TODO: Add Description**|
|appRoles|[appRole](../resources/microsoft.directoryservices-approle.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|errorUrl|String|**TODO: Add Description**|
|hasPermissionClassifications|Boolean|**TODO: Add Description**|
|homepage|String|**TODO: Add Description**|
|info|[informationalUrl](../resources/microsoft.directoryservices-informationalurl.md)|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/microsoft.directoryservices-keycredential.md) collection|**TODO: Add Description**|
|loginUrl|String|**TODO: Add Description**|
|logoutUrl|String|**TODO: Add Description**|
|notificationEmailAddresses|String collection|**TODO: Add Description**|
|publishedPermissionScopes|[permissionScope](../resources/microsoft.directoryservices-permissionscope.md) collection|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/microsoft.directoryservices-passwordcredential.md) collection|**TODO: Add Description**|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|**TODO: Add Description**|
|preferredTokenSigningKeyThumbprint|String|**TODO: Add Description**|
|preferredSingleSignOnMode|String|**TODO: Add Description**|
|publisherName|String|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|
|samlMetadataUrl|String|**TODO: Add Description**|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/microsoft.directoryservices-samlsinglesignonsettings.md)|**TODO: Add Description**|
|servicePrincipalNames|String collection|**TODO: Add Description**|
|servicePrincipalType|String|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [servicePrincipal](../resources/microsoft.directoryservices-serviceprincipal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}
-->
``` http
POST https://graph.microsoft.com/changelog/servicePrincipals
Content-Type: application/json
Content-length: 3939

{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipal",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "Microsoft.DirectoryServices.addIn",
      "id": "6ce1b2dc-b2dc-6ce1-dcb2-e16cdcb2e16c",
      "type": "Type value",
      "properties": [
        {
          "@odata.type": "Microsoft.DirectoryServices.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ]
    }
  ],
  "alternativeNames": [
    "Alternative Names value"
  ],
  "api": {
    "@odata.type": "Microsoft.DirectoryServices.apiServicePrincipal",
    "resourceSpecificApplicationPermissions": [
      {
        "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
        "description": "Description value",
        "displayName": "Display Name value",
        "isEnabled": true
      }
    ]
  },
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "applicationTemplateId": "Application Template Id value",
  "appOwnerOrganizationId": "645cf9c9-f9c9-645c-c9f9-5c64c9f95c64",
  "appRoleAssignmentRequired": true,
  "appRoles": [
    {
      "@odata.type": "Microsoft.DirectoryServices.appRole",
      "allowedMemberTypes": [
        "Allowed Member Types value"
      ],
      "origin": "Origin value"
    }
  ],
  "displayName": "Display Name value",
  "errorUrl": "https://example.com/errorUrl/",
  "hasPermissionClassifications": true,
  "homepage": "Homepage value",
  "info": {
    "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
    "logoUrl": "https://example.com/logoUrl/",
    "marketingUrl": "https://example.com/marketingUrl/",
    "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
    "supportUrl": "https://example.com/supportUrl/",
    "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
  },
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
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
      "@odata.type": "Microsoft.DirectoryServices.permissionScope",
      "adminConsentDescription": "Admin Consent Description value",
      "adminConsentDisplayName": "Admin Consent Display Name value",
      "userConsentDescription": "User Consent Description value",
      "userConsentDisplayName": "User Consent Display Name value"
    }
  ],
  "passwordCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
      "secretText": "Secret Text value",
      "hint": "Hint value"
    }
  ],
  "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:36.1296382+00:00",
  "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
  "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
  "publisherName": "Publisher Name value",
  "replyUrls": [
    "Reply Urls value"
  ],
  "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
  "samlSingleSignOnSettings": {
    "@odata.type": "Microsoft.DirectoryServices.samlSingleSignOnSettings",
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
  "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.serviceprincipal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipal",
  "id": "f1245539-5539-f124-3955-24f1395524f1",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "accountEnabled": true,
  "addIns": [
    {
      "@odata.type": "Microsoft.DirectoryServices.addIn",
      "id": "6ce1b2dc-b2dc-6ce1-dcb2-e16cdcb2e16c",
      "type": "Type value",
      "properties": [
        {
          "@odata.type": "Microsoft.DirectoryServices.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ]
    }
  ],
  "alternativeNames": [
    "Alternative Names value"
  ],
  "api": {
    "@odata.type": "Microsoft.DirectoryServices.apiServicePrincipal",
    "resourceSpecificApplicationPermissions": [
      {
        "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
        "description": "Description value",
        "displayName": "Display Name value",
        "isEnabled": true
      }
    ]
  },
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "applicationTemplateId": "Application Template Id value",
  "appOwnerOrganizationId": "645cf9c9-f9c9-645c-c9f9-5c64c9f95c64",
  "appRoleAssignmentRequired": true,
  "appRoles": [
    {
      "@odata.type": "Microsoft.DirectoryServices.appRole",
      "allowedMemberTypes": [
        "Allowed Member Types value"
      ],
      "origin": "Origin value"
    }
  ],
  "displayName": "Display Name value",
  "errorUrl": "https://example.com/errorUrl/",
  "hasPermissionClassifications": true,
  "homepage": "Homepage value",
  "info": {
    "@odata.type": "Microsoft.DirectoryServices.informationalUrl",
    "logoUrl": "https://example.com/logoUrl/",
    "marketingUrl": "https://example.com/marketingUrl/",
    "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
    "supportUrl": "https://example.com/supportUrl/",
    "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
  },
  "keyCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.keyCredential",
      "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
      "endDateTime": "2017-01-01T00:01:58.2456509+00:00",
      "keyId": "c4860b27-0b27-c486-270b-86c4270b86c4",
      "startDateTime": "2017-01-01T00:01:26.5340071+00:00",
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
      "@odata.type": "Microsoft.DirectoryServices.permissionScope",
      "adminConsentDescription": "Admin Consent Description value",
      "adminConsentDisplayName": "Admin Consent Display Name value",
      "userConsentDescription": "User Consent Description value",
      "userConsentDisplayName": "User Consent Display Name value"
    }
  ],
  "passwordCredentials": [
    {
      "@odata.type": "Microsoft.DirectoryServices.passwordCredential",
      "secretText": "Secret Text value",
      "hint": "Hint value"
    }
  ],
  "preferredTokenSigningKeyEndDateTime": "2016-12-31T23:59:36.1296382+00:00",
  "preferredTokenSigningKeyThumbprint": "Preferred Token Signing Key Thumbprint value",
  "preferredSingleSignOnMode": "Preferred Single Sign On Mode value",
  "publisherName": "Publisher Name value",
  "replyUrls": [
    "Reply Urls value"
  ],
  "samlMetadataUrl": "https://example.com/samlMetadataUrl/",
  "samlSingleSignOnSettings": {
    "@odata.type": "Microsoft.DirectoryServices.samlSingleSignOnSettings",
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
  "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99"
}
```

