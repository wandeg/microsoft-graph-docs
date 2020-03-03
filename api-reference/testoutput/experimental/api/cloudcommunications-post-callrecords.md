---
title: "Add callRecords"
description: "Add callRecords by posting to the callRecords collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add callRecords

Namespace: microsoft.graph.callRecords

Add callRecords by posting to the callRecords collection.

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
POST /communications/callRecords/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [callRecord](../resources/callrecords-callrecord.md) object.

The following table shows the properties that are required when you create the [callRecord](../resources/callrecords-callrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|version|Int64||
|type|Enumeration|. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|modalities|Enumeration collection|. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|organizer|[identitySet](../resources/callrecords-identityset.md)||
|participants|[identitySet](../resources/callrecords-identityset.md) collection||
|joinWebUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [callRecord](../resources/callrecords-callrecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_callrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/callRecords
Content-type: application/json
Content-length: 766

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "joinWebUrl": "https://example.com/joinWebUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.callrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 879

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "319f7649-7649-319f-4976-9f3149769f31",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "joinWebUrl": "https://example.com/joinWebUrl/"
}
```

