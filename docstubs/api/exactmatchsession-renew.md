---
title: "renew"
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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "exactmatchsession_renew"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions/{exactMatchSessionId}/renew
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactmatchsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1031

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchSession",
    "id": "fe1acbc8-cbc8-fe1a-c8cb-1afec8cb1afe",
    "creationDateTime": "2016-12-31T23:57:30.6368517+03:00",
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "lastUpdatedDateTime": "2016-12-31T23:57:43.3634504+03:00",
    "completionDateTime": "2017-01-01T00:01:29.1253152+03:00",
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
    "uploadCompletionDateTime": "2016-12-31T23:58:05.9642398+03:00",
    "processingCompletionDateTime": "2017-01-01T00:01:51.4896431+03:00",
    "rowsPerBlock": 12,
    "totalJobCount": 13,
    "remainingJobCount": 1
  }
}
```

