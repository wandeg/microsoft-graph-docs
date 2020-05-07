---
title: "Get provisioningObjectSummary"
description: "Read the properties and relationships of a provisioningObjectSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get provisioningObjectSummary

Namespace: microsoft.graph

Read the properties and relationships of a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

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
GET /auditLogs/provisioning/{provisioningObjectSummaryId}
GET /auditLogs/directoryProvisioning/{provisioningObjectSummaryId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/provisioning/{provisioningObjectSummaryId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.provisioningObjectSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.provisioningObjectSummary",
    "id": "1889eaac-eaac-1889-acea-8918acea8918",
    "activityDateTime": "String (timestamp)",
    "tenantId": "String",
    "jobId": "String",
    "cycleId": "String",
    "changeId": "String",
    "action": "String",
    "durationInMilliseconds": "Integer",
    "servicePrincipal": {
      "@odata.type": "microsoft.graph.provisioningServicePrincipal"
    },
    "initiatedBy": {
      "@odata.type": "microsoft.graph.initiator"
    },
    "sourceSystem": {
      "@odata.type": "microsoft.graph.provisioningSystemDetails"
    },
    "targetSystem": {
      "@odata.type": "microsoft.graph.provisioningSystemDetails"
    },
    "sourceIdentity": {
      "@odata.type": "microsoft.graph.provisionedIdentity"
    },
    "targetIdentity": {
      "@odata.type": "microsoft.graph.provisionedIdentity"
    },
    "statusInfo": {
      "@odata.type": "microsoft.graph.statusBase"
    },
    "provisioningSteps": [
      {
        "@odata.type": "microsoft.graph.provisioningStep"
      }
    ],
    "modifiedProperties": [
      {
        "@odata.type": "microsoft.graph.modifiedProperty"
      }
    ]
  }
}
```

