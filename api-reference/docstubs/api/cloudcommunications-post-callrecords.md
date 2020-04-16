---
title: "Create callRecords"
description: "Create a new callRecords object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create callRecords

Namespace: microsoft.graph.callRecords

Create a new callRecords object.

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
POST /communications/callRecords
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [callRecord](../resources/callrecords-callrecord.md) object.

The following table shows the properties that are required when you create the [callRecord](../resources/callrecords-callrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md)|
|version|Int64|**TODO: Add Description**|
|type|callType|**TODO: Add Description**. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|modalities|modality collection|**TODO: Add Description**. Possible values are: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|organizer|[identitySet](../resources/callrecords-identityset.md)|**TODO: Add Description**|
|participants|[identitySet](../resources/callrecords-identityset.md) collection|**TODO: Add Description**|
|joinWebUrl|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [callRecord](../resources/callrecords-callrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_callrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/callRecords
Content-Type: application/json
Content-length: 766

{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "startDateTime": "2017-01-01T00:01:28.8507081+03:00",
  "endDateTime": "2017-01-01T00:02:50.4198958+03:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.callrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "3e424108-4108-3e42-0841-423e0841423e",
  "version": 7,
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "2016-12-31T23:56:35.1491722+03:00",
  "startDateTime": "2017-01-01T00:01:28.8507081+03:00",
  "endDateTime": "2017-01-01T00:02:50.4198958+03:00",
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

