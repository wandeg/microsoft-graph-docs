---
title: "Add appLogCollectionRequests"
description: "Add appLogCollectionRequests by posting to the appLogCollectionRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appLogCollectionRequests

Namespace: microsoft.graph

Add appLogCollectionRequests by posting to the appLogCollectionRequests collection.

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
POST /me/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/applogcollectionrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_applogcollectionrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
Content-type: application/json
Content-length: 254

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "String",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2017-01-01T00:01:28.4865953+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applogcollectionrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 303

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "136fa1af-a1af-136f-afa1-6f13afa16f13",
  "status": "String",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2017-01-01T00:01:28.4865953+03:00"
}
```

