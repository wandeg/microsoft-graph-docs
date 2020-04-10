---
title: "exactMatchSession: renew"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# renew

Namespace: microsoft.graph



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
POST /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/renew
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [exactMatchSession](../resources/exactmatchsession.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "exactmatchsession_renew"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/renew
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1058

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchSession",
    "id": "b84d3f36-3f36-b84d-363f-4db8363f4db8",
    "creationDateTime": "2017-01-01T00:02:38.3339201+00:00",
    "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
    "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00",
    "completionDateTime": "2016-12-31T23:58:05.4513555+00:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "datastoreId": "Datastore Id value",
    "uploadAgentId": "Upload Agent Id value",
    "fields": [
      "Fields value"
    ],
    "fileName": "File Name value",
    "checksum": "Checksum value",
    "dataUploadURI": "Data Upload URI value",
    "remainingBlockCount": 3,
    "totalBlockCount": 15,
    "state": "State value",
    "uploadCompletionDateTime": "2017-01-01T00:02:05.8475063+00:00",
    "processingCompletionDateTime": "2017-01-01T00:01:57.0595644+00:00",
    "rowsPerBlock": 12,
    "totalJobCount": 13,
    "remainingJobCount": 1,
    "salt": "Salt value"
  }
}
```

