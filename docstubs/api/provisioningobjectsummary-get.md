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
|Name|Description|
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
GET https://graph.microsoft.com/beta/auditLogs/provisioning/{provisioningObjectSummaryId}
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
Content-Length: 1732

{
  "value": {
    "@odata.type": "#microsoft.graph.provisioningObjectSummary",
    "id": "d253e006-e006-d253-06e0-53d206e053d2",
    "activityDateTime": "2017-01-01T00:01:00.3600822+03:00",
    "tenantId": "Tenant Id value",
    "jobId": "Job Id value",
    "cycleId": "Cycle Id value",
    "changeId": "Change Id value",
    "action": "Action value",
    "durationInMilliseconds": 6,
    "servicePrincipal": {
      "@odata.type": "microsoft.graph.provisioningServicePrincipal",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "initiatedBy": {
      "@odata.type": "microsoft.graph.initiator",
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

