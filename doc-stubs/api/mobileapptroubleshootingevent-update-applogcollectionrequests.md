---
title: "Update appLogCollectionRequests"
description: "Update the properties of an appLogCollectionRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update appLogCollectionRequests

Namespace: microsoft.graph

Update the properties of an appLogCollectionRequests object.

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
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.

The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/applogcollectionrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|appLogUploadState|**TODO: Add Description**. Possible values are: `pending`, `completed`, `failed`.|
|errorMessage|String|**TODO: Add Description**|
|customLogFolders|String collection|**TODO: Add Description**|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/applogcollectionrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applogcollectionrequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
Content-Type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "56615e4b-5e4b-5661-4b5e-61564b5e6156",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```

