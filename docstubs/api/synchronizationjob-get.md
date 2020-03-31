---
title: "Get synchronizationJob"
description: "Read properties and relationships of the synchronizationJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get synchronizationJob

Namespace: microsoft.graph

Read properties and relationships of the [synchronizationJob](../resources/synchronizationjob.md) object.

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
GET /applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
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
If successful, this method returns a `200 OK` response code and [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs/{synchronizationJobId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2877

{
  "value": {
    "@odata.type": "#microsoft.graph.synchronizationJob",
    "id": "2065f624-f624-2065-24f6-652024f66520",
    "templateId": "Template Id value",
    "schedule": {
      "@odata.type": "microsoft.graph.synchronizationSchedule",
      "expiration": "2016-12-31T23:57:39.0449164+03:00",
      "interval": "-PT29.468746S",
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
        "timeBegan": "2017-01-01T00:03:20.5651763+03:00",
        "timeEnded": "2016-12-31T23:56:42.848301+03:00"
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
          "progressObservationDateTime": "2016-12-31T23:56:56.4898767+03:00",
          "totalUnits": 10,
          "units": "Units value"
        }
      ],
      "quarantine": {
        "@odata.type": "microsoft.graph.synchronizationQuarantine",
        "currentBegan": "2016-12-31T23:59:29.1455514+03:00",
        "nextAttempt": "2017-01-01T00:00:49.370262+03:00",
        "reason": "String",
        "seriesBegan": "2017-01-01T00:01:06.4363322+03:00",
        "seriesCount": 11
      },
      "steadyStateFirstAchievedTime": "2016-12-31T23:58:12.5314275+03:00",
      "steadyStateLastAchievedTime": "2016-12-31T23:59:45.2733216+03:00",
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
}
```

