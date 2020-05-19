---
title: "List windowsInformationProtectionPolicies"
description: "Get the windowsInformationProtectionPolicies from the windowsInformationProtectionPolicies navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List windowsInformationProtectionPolicies

Namespace: microsoft.graph

Get the windowsInformationProtectionPolicies from the windowsInformationProtectionPolicies navigation property.

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
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectionpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsinformationprotectionpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "id": "28662993-2993-2866-9329-662893296628",
      "displayName": "String",
      "description": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
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
      "isAssigned": "Boolean",
      "revokeOnMdmHandoffDisabled": "Boolean",
      "mdmEnrollmentUrl": "String",
      "windowsHelloForBusinessBlocked": "Boolean",
      "pinMinimumLength": "Integer",
      "pinUppercaseLetters": "String",
      "pinLowercaseLetters": "String",
      "pinSpecialCharacters": "String",
      "pinExpirationDays": "Integer",
      "numberOfPastPinsRemembered": "Integer",
      "passwordMaximumAttemptCount": "Integer",
      "minutesOfInactivityBeforeDeviceLock": "Integer",
      "daysWithoutContactBeforeUnenroll": "Integer"
    }
  ]
}
```

