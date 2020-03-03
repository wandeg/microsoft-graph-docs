---
title: "Update mobileAppContentFile"
description: "Update the properties of a mobileAppContentFile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mobileAppContentFile

Namespace: microsoft.graph

Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.

The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|azureStorageUri|String|The Azure Storage URI.|
|isCommitted|Boolean|A value indicating whether the file is committed.|
|createdDateTime|DateTimeOffset|The time the file was created.|
|name|String|the file name.|
|size|Int64|The size of the file prior to encryption.|
|sizeEncrypted|Int64|The size of the file after encryption.|
|azureStorageUriExpirationDateTime|DateTimeOffset|The time the Azure storage Uri expires.|
|manifest|Binary|The manifest information.|
|uploadState|Enumeration|The state of the current upload request. Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|
|isFrameworkFile|Boolean|A value indicating whether the file is a framework file.|
|isDependency|Boolean|Whether the content file is a dependency for the main content file.|



## Response
If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mobileappcontentfile"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:02:49.8360031+03:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
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
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "id": "fbfff66f-f66f-fbff-6ff6-fffb6ff6fffb",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:02:49.8360031+03:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```

