---
title: "List provisioning"
description: "Get the provisioningObjectSummaries from the provisioning navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List provisioning

Namespace: Microsoft.AAD.Reporting

Get the provisioningObjectSummaries from the provisioning navigation property.

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
GET /auditLogs/provisioning
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aad.reporting.provisioningobjectsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
      "id": "1af8a3ef-a3ef-1af8-efa3-f81aefa3f81a",
      "activityDateTime": "2017-01-01T00:03:11.0875532+00:00",
      "tenantId": "Tenant Id value",
      "jobId": "Job Id value",
      "cycleId": "Cycle Id value",
      "changeId": "Change Id value",
      "action": "Action value",
      "durationInMilliseconds": 6,
      "servicePrincipal": {
        "@odata.type": "Microsoft.AAD.Reporting.provisioningServicePrincipal",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "initiatedBy": {
        "@odata.type": "Microsoft.AAD.Reporting.initiator",
        "initiatorType": "String"
      },
      "sourceSystem": {
        "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails",
        "details": {
          "@odata.type": "Microsoft.AAD.Reporting.detailsInfo"
        }
      },
      "targetSystem": {
        "@odata.type": "Microsoft.AAD.Reporting.provisioningSystemDetails"
      },
      "sourceIdentity": {
        "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity",
        "identityType": "Identity Type value"
      },
      "targetIdentity": {
        "@odata.type": "Microsoft.AAD.Reporting.provisionedIdentity"
      },
      "statusInfo": {
        "@odata.type": "Microsoft.AAD.Reporting.statusBase",
        "status": "String"
      },
      "provisioningSteps": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.provisioningStep",
          "name": "Name value",
          "description": "Description value",
          "provisioningStepType": "String"
        }
      ],
      "modifiedProperties": [
        {
          "@odata.type": "Microsoft.AAD.Reporting.modifiedProperty",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ]
    }
  ]
}
```

