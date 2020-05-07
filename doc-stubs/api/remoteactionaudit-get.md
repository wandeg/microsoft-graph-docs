---
title: "Get remoteActionAudit"
description: "Read the properties and relationships of a remoteActionAudit object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get remoteActionAudit

Namespace: microsoft.graph

Read the properties and relationships of a [remoteActionAudit](../resources/remoteactionaudit.md) object.

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
GET /deviceManagement/remoteActionAudits/{remoteActionAuditId}
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

If successful, this method returns a `200 OK` response code and a [remoteActionAudit](../resources/remoteactionaudit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_remoteactionaudit"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.remoteActionAudit",
    "id": "4f916c32-6c32-4f91-326c-914f326c914f",
    "deviceDisplayName": "String",
    "userName": "String",
    "initiatedByUserPrincipalName": "String",
    "action": "String",
    "requestDateTime": "String (timestamp)",
    "deviceOwnerUserPrincipalName": "String",
    "deviceIMEI": "String",
    "actionState": "String",
    "managedDeviceId": "String"
  }
}
```

