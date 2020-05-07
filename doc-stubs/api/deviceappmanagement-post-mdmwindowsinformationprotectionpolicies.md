---
title: "Create mdmWindowsInformationProtectionPolicies"
description: "Create a new mdmWindowsInformationProtectionPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create mdmWindowsInformationProtectionPolicies

Namespace: microsoft.graph

Create a new mdmWindowsInformationProtectionPolicies object.

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
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object.

The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/windowsinformationprotectiondatarecoverycertificate.md)|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|revokeOnUnenrollDisabled|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|azureRightsManagementServicesAllowed|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|iconsVisible|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/windowsinformationprotectionproxieddomaincollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/windowsinformationprotectioniprangecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|isAssigned|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|



## Response

If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/mdmwindowsinformationprotectionpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mdmwindowsinformationprotectionpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-Type: application/json
Content-length: 2185

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "protectionUnderLockConfigRequired": "Boolean",
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
  },
  "revokeOnUnenrollDisabled": "Boolean",
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": "Boolean",
  "iconsVisible": "Boolean",
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
    }
  ],
  "enterpriseIPRangesAreAuthoritative": "Boolean",
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxyServersAreAuthoritative": "Boolean",
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": "Boolean",
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "isAssigned": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mdmwindowsinformationprotectionpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "id": "e56f33c0-33c0-e56f-c033-6fe5c0336fe5",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "protectionUnderLockConfigRequired": "Boolean",
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
  },
  "revokeOnUnenrollDisabled": "Boolean",
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": "Boolean",
  "iconsVisible": "Boolean",
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
    }
  ],
  "enterpriseIPRangesAreAuthoritative": "Boolean",
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxyServersAreAuthoritative": "Boolean",
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": "Boolean",
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "isAssigned": "Boolean"
}
```

