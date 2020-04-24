---
title: "List remoteActionAudits"
description: "Get the remoteActionAudits from the remoteActionAudits navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List remoteActionAudits

Namespace: microsoft.graph

Get the remoteActionAudits from the remoteActionAudits navigation property.

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
GET /deviceManagement/remoteActionAudits
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
If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/remoteactionaudit.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_remoteactionaudit"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.remoteactionaudit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteActionAudit",
      "id": "ee2db833-b833-ee2d-33b8-2dee33b82dee",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
      "action": "String",
      "requestDateTime": "2017-01-01T00:02:26.8557697+03:00",
      "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
      "deviceIMEI": "Device IMEI value",
      "actionState": "String",
      "managedDeviceId": "Managed Device Id value"
    }
  ]
}
```

