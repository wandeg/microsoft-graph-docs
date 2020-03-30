---
title: "List sessions"
description: "Get the exactMatchSessions from the sessions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sessions

Namespace: microsoft.graph

Get the exactMatchSessions from the sessions navigation property.

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
GET /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [exactMatchSession](../resources/exactmatchsession.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchsession"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}/sessions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchsession)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.exactMatchSession",
      "id": "574611a9-11a9-5746-a911-4657a9114657",
      "creationDateTime": "2016-12-31T23:59:06.3080317+03:00",
      "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:59:55.7493178+03:00",
      "completionDateTime": "2017-01-01T00:01:17.3860037+03:00",
      "error": {
        "@odata.type": "microsoft.graph.classificationError",
        "code": "Code value",
        "message": "Message value",
        "target": "Target value",
        "innerError": {
          "@odata.type": "microsoft.graph.classificationInnerError",
          "errorDateTime": "2017-01-01T00:03:31.1650712+03:00",
          "clientRequestId": "Client Request Id value",
          "activityId": "Activity Id value"
        },
        "details": [
          {
            "@odata.type": "microsoft.graph.classifcationErrorBase"
          }
        ]
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
      "uploadCompletionDateTime": "2016-12-31T23:57:53.2214037+03:00",
      "processingCompletionDateTime": "2016-12-31T23:58:03.4123227+03:00",
      "rowsPerBlock": 12,
      "totalJobCount": 13,
      "remainingJobCount": 1
    }
  ]
}
```

