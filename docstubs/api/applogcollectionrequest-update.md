---
title: "Update appLogCollectionRequest"
description: "Update the properties of a appLogCollectionRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update appLogCollectionRequest

Namespace: microsoft.graph

Update the properties of a [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.

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
PATCH /me/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/applogcollectionrequest.md) object.

The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/applogcollectionrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `pending`, `completed`, `failed`.|
|errorMessage|String||
|customLogFolders|String collection||
|completedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/applogcollectionrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_applogcollectionrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 254

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "String",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2017-01-01T00:03:18.4386811+00:00"
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
Content-Length: 303

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "d1ec59f1-59f1-d1ec-f159-ecd1f159ecd1",
  "status": "String",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2017-01-01T00:03:18.4386811+00:00"
}
```

