---
title: "Update provisioning"
description: "Update the properties of a provisioning object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update provisioning

Namespace: microsoft.graph

Update the properties of a provisioning object.

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
PATCH /auditLogs/provisioning
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object.

The following table shows the properties that are required when you create the [provisioningObjectSummary](../resources/provisioningobjectsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|jobId|String|**TODO: Add Description**|
|cycleId|String|**TODO: Add Description**|
|changeId|String|**TODO: Add Description**|
|action|String|**TODO: Add Description**|
|durationInMilliseconds|Int32|**TODO: Add Description**|
|servicePrincipal|[provisioningServicePrincipal](../resources/provisioningserviceprincipal.md)|**TODO: Add Description**|
|initiatedBy|[initiator](../resources/initiator.md)|**TODO: Add Description**|
|sourceSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|targetSystem|[provisioningSystemDetails](../resources/provisioningsystemdetails.md)|**TODO: Add Description**|
|sourceIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|targetIdentity|[provisionedIdentity](../resources/provisionedidentity.md)|**TODO: Add Description**|
|statusInfo|[statusBase](../resources/statusbase.md)|**TODO: Add Description**|
|provisioningSteps|[provisioningStep](../resources/provisioningstep.md) collection|**TODO: Add Description**|
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [provisioningObjectSummary](../resources/provisioningobjectsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_provisioning"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/provisioning
Content-Type: application/json
Content-length: 1558

{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.provisioningObjectSummary",
  "id": "c094201e-201e-c094-1e20-94c01e2094c0",
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
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
```

