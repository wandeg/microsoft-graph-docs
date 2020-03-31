---
title: "List jobs"
description: "Get the synchronizationJobs from the jobs navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List jobs

Namespace: microsoft.graph

Get the synchronizationJobs from the jobs navigation property.

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
GET /applications/{applicationsId}/synchronization/jobs
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
If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronizationjob.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.synchronizationjob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3046

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.synchronizationJob",
      "id": "e0cb1c1d-1c1d-e0cb-1d1c-cbe01d1ccbe0",
      "templateId": "Template Id value",
      "schedule": {
        "@odata.type": "microsoft.graph.synchronizationSchedule",
        "expiration": "2017-01-01T00:03:28.2449648+03:00",
        "interval": "-PT23.6405647S",
        "state": "String"
      },
      "status": {
        "@odata.type": "microsoft.graph.synchronizationStatus",
        "countSuccessiveCompleteFailures": 15,
        "escrowsPruned": true,
        "code": "String",
        "lastExecution": {
          "@odata.type": "microsoft.graph.synchronizationTaskExecution",
          "activityIdentifier": "Activity Identifier value",
          "countEntitled": 13,
          "countEntitledForProvisioning": 12,
          "countEscrowed": 13,
          "countEscrowedRaw": 0,
          "countExported": 13,
          "countExports": 12,
          "countImported": 13,
          "countImportedDeltas": 3,
          "countImportedReferenceDeltas": 12,
          "state": "String",
          "error": {
            "@odata.type": "microsoft.graph.synchronizationError",
            "code": "Code value",
            "message": "Message value",
            "tenantActionable": true
          },
          "timeBegan": "2016-12-31T23:56:53.1182443+03:00",
          "timeEnded": "2017-01-01T00:03:19.7463735+03:00"
        },
        "lastSuccessfulExecution": {
          "@odata.type": "microsoft.graph.synchronizationTaskExecution"
        },
        "lastSuccessfulExecutionWithExports": {
          "@odata.type": "microsoft.graph.synchronizationTaskExecution"
        },
        "progress": [
          {
            "@odata.type": "microsoft.graph.synchronizationProgress",
            "completedUnits": 14,
            "progressObservationDateTime": "2016-12-31T23:59:02.92446+03:00",
            "totalUnits": 10,
            "units": "Units value"
          }
        ],
        "quarantine": {
          "@odata.type": "microsoft.graph.synchronizationQuarantine",
          "currentBegan": "2017-01-01T00:02:46.9898752+03:00",
          "nextAttempt": "2016-12-31T23:56:56.2333948+03:00",
          "reason": "String",
          "seriesBegan": "2016-12-31T23:57:57.5024003+03:00",
          "seriesCount": 11
        },
        "steadyStateFirstAchievedTime": "2016-12-31T23:58:23.0731642+03:00",
        "steadyStateLastAchievedTime": "2016-12-31T23:56:51.2015398+03:00",
        "synchronizedEntryCountByType": [
          {
            "@odata.type": "microsoft.graph.stringKeyLongValuePair",
            "key": "Key value",
            "value": 5
          }
        ],
        "troubleshootingUrl": "https://example.com/troubleshootingUrl/"
      },
      "synchronizationJobSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

