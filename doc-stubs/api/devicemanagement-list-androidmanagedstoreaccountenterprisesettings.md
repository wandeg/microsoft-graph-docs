---
title: "List androidManagedStoreAccountEnterpriseSettings"
description: "Get the androidManagedStoreAccountEnterpriseSettings from the androidManagedStoreAccountEnterpriseSettings navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List androidManagedStoreAccountEnterpriseSettings

Namespace: microsoft.graph

Get the androidManagedStoreAccountEnterpriseSettings from the androidManagedStoreAccountEnterpriseSettings navigation property.

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
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
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

If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAccountEnterpriseSettings](../resources/androidmanagedstoreaccountenterprisesettings.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androidmanagedstoreaccountenterprisesettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.androidmanagedstoreaccountenterprisesettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
      "id": "32e582d9-82d9-32e5-d982-e532d982e532",
      "bindStatus": "String",
      "lastAppSyncDateTime": "String (timestamp)",
      "lastAppSyncStatus": "String",
      "ownerUserPrincipalName": "String",
      "ownerOrganizationName": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "enrollmentTarget": "String",
      "targetGroupIds": [
        "String"
      ],
      "deviceOwnerManagementEnabled": "Boolean",
      "companyCodes": [
        {
          "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
        }
      ],
      "androidDeviceOwnerFullyManagedEnrollmentEnabled": "Boolean"
    }
  ]
}
```

