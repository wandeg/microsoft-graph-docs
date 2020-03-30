---
title: "Add jobs"
description: "Add jobs by posting to the jobs collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add jobs

Namespace: microsoft.graph

Add jobs by posting to the jobs collection.

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
POST /applications/{applicationsId}/synchronization/jobs/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [synchronizationJob](../resources/synchronizationjob.md) object.

The following table shows the properties that are required when you create the [synchronizationJob](../resources/synchronizationjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|templateId|String||
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)||
|status|[synchronizationStatus](../resources/synchronizationstatus.md)||
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/jobs
Content-type: application/json
Content-length: 2659

{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "templateId": "Template Id value",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule",
    "expiration": "2017-01-01T00:02:27.2449657+00:00",
    "interval": "-PT2M33.9901443S",
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
      "timeBegan": "2016-12-31T23:59:52.5766771+00:00",
      "timeEnded": "2016-12-31T23:58:14.4260137+00:00"
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
        "progressObservationDateTime": "2016-12-31T23:59:31.4783051+00:00",
        "totalUnits": 10,
        "units": "Units value"
      }
    ],
    "quarantine": {
      "@odata.type": "microsoft.graph.synchronizationQuarantine",
      "currentBegan": "2016-12-31T23:59:48.3779097+00:00",
      "nextAttempt": "2017-01-01T00:02:57.7620496+00:00",
      "reason": "String",
      "seriesBegan": "2016-12-31T23:58:25.194102+00:00",
      "seriesCount": 11
    },
    "steadyStateFirstAchievedTime": "2017-01-01T00:03:24.4754618+00:00",
    "steadyStateLastAchievedTime": "2016-12-31T23:56:36.4334018+00:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationjob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2708

{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "c8bf891e-891e-c8bf-1e89-bfc81e89bfc8",
  "templateId": "Template Id value",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule",
    "expiration": "2017-01-01T00:02:27.2449657+00:00",
    "interval": "-PT2M33.9901443S",
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
      "timeBegan": "2016-12-31T23:59:52.5766771+00:00",
      "timeEnded": "2016-12-31T23:58:14.4260137+00:00"
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
        "progressObservationDateTime": "2016-12-31T23:59:31.4783051+00:00",
        "totalUnits": 10,
        "units": "Units value"
      }
    ],
    "quarantine": {
      "@odata.type": "microsoft.graph.synchronizationQuarantine",
      "currentBegan": "2016-12-31T23:59:48.3779097+00:00",
      "nextAttempt": "2017-01-01T00:02:57.7620496+00:00",
      "reason": "String",
      "seriesBegan": "2016-12-31T23:58:25.194102+00:00",
      "seriesCount": 11
    },
    "steadyStateFirstAchievedTime": "2017-01-01T00:03:24.4754618+00:00",
    "steadyStateLastAchievedTime": "2016-12-31T23:56:36.4334018+00:00",
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
```

