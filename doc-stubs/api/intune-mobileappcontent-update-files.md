---
title: "Update files"
description: "Update the properties of a files object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update files

Namespace: microsoft.graph

Update the properties of a files object.

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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobileAppContentFile](../resources/intune-mobileappcontentfile.md) object.

The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-mobileappcontentfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|azureStorageUri|String|**TODO: Add Description**|
|isCommitted|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|size|Int64|**TODO: Add Description**|
|sizeEncrypted|Int64|**TODO: Add Description**|
|azureStorageUriExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|manifest|Binary|**TODO: Add Description**|
|uploadState|mobileAppContentFileUploadState|**TODO: Add Description**. Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-mobileappcontentfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_files"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-Type: application/json
Content-length: 312

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": "Boolean",
  "name": "String",
  "size": "Integer",
  "sizeEncrypted": "Integer",
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "Binary",
  "uploadState": "String"
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
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "id": "7461dd80-dd80-7461-80dd-617480dd6174",
  "azureStorageUri": "String",
  "isCommitted": "Boolean",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": "Integer",
  "sizeEncrypted": "Integer",
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "Binary",
  "uploadState": "String"
}
```

