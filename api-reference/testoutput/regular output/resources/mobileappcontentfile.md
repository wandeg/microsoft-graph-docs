---
title: "mobileAppContentFile resource type"
description: "Contains properties for a single installer file that is associated with a given mobileAppContent version."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mobileAppContentFile resource type

Contains properties for a single installer file that is associated with a given mobileAppContent version.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppContentFile](../api/mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md)|Read properties and relationships of the [mobileAppContentFile](../resources/mobileappcontentfile.md) object.|
|[Delete mobileAppContentFile](../api/mobileappcontentfile-delete.md)|None|Deletes a [mobileAppContentFile](../resources/mobileappcontentfile.md).|
|[Update mobileAppContentFile](../api/mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md)|Update the properties of a [mobileAppContentFile](../resources/mobileappcontentfile.md) object.|
|[commit](../api/mobileappcontentfile-commit.md)|None||
|[renewUpload](../api/mobileappcontentfile-renewupload.md)|None||
|[List files](../api/mobileappcontent-list-files.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md) collection|Get the mobileAppContentFiles from the files navigation property.|
|[Add files](../api/mobileappcontent-post-files.md)|[mobileAppContentFile](../resources/mobileAppContentFile.md)|Add files by posting to the files collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureStorageUri|String|The Azure Storage URI.|
|azureStorageUriExpirationDateTime|DateTimeOffset|The time the Azure storage Uri expires.|
|createdDateTime|DateTimeOffset|The time the file was created.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isCommitted|Boolean|A value indicating whether the file is committed.|
|manifest|Binary|The manifest information.|
|name|String|the file name.|
|size|Int64|The size of the file prior to encryption.|
|sizeEncrypted|Int64|The size of the file after encryption.|
|uploadState|Enumeration|The state of the current upload request. Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "id": "String (identifier)",
  "azureStorageUri": "String",
  "isCommitted": true,
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```

