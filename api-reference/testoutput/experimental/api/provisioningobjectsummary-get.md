---
title: "Get provisioningObjectSummary"
description: "Read properties and relationships of the provisioningObjectSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get provisioningObjectSummary

Namespace: microsoft.graph

Read properties and relationships of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

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
GET /auditLogs/provisioning/{provisioningObjectSummaryId}
GET /auditLogs/directoryProvisioning/{provisioningObjectSummaryId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/provisioning/{provisioningObjectSummaryId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1628

{
  "value": {
    "@odata.type": "#microsoft.graph.provisioningObjectSummary",
    "id": "f1007e49-7e49-f100-497e-00f1497e00f1",
    "activityDateTime": "2016-12-31T23:56:58.7486077+03:00",
    "tenantId": "Tenant Id value",
    "jobId": "Job Id value",
    "cycleId": "Cycle Id value",
    "changeId": "Change Id value",
    "action": "Action value",
    "durationInMilliseconds": 6,
    "initiatedBy": {
      "@odata.type": "microsoft.graph.initiator",
      "id": "Id value",
      "displayName": "Display Name value",
      "initiatorType": "String"
    },
    "sourceSystem": {
      "@odata.type": "microsoft.graph.provisioningSystemDetails",
      "details": {
        "@odata.type": "microsoft.graph.detailsInfo"
      }
    },
    "targetSystem": {
      "@odata.type": "microsoft.graph.provisioningSystemDetails"
    },
    "sourceIdentity": {
      "@odata.type": "microsoft.graph.provisionedIdentity",
      "identityType": "Identity Type value"
    },
    "targetIdentity": {
      "@odata.type": "microsoft.graph.provisionedIdentity"
    },
    "statusInfo": {
      "@odata.type": "microsoft.graph.statusBase",
      "status": "String"
    },
    "provisioningSteps": [
      {
        "@odata.type": "microsoft.graph.provisioningStep",
        "name": "Name value",
        "description": "Description value",
        "provisioningStepType": "String"
      }
    ],
    "modifiedProperties": [
      {
        "@odata.type": "microsoft.graph.modifiedProperty",
        "oldValue": "Old Value value",
        "newValue": "New Value value"
      }
    ]
  }
}
```

