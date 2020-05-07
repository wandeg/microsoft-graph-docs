---
title: "Update domainJoinConnectors"
description: "Update the properties of a domainJoinConnectors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update domainJoinConnectors

Namespace: microsoft.graph

Update the properties of a domainJoinConnectors object.

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
PATCH /deviceManagement/domainJoinConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|lastConnectionDateTime|DateTimeOffset|**TODO: Add Description**|
|state|deviceManagementDomainJoinConnectorState|**TODO: Add Description**. Possible values are: `active`, `error`, `inactive`.|
|version|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/devicemanagementdomainjoinconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_domainjoinconnectors"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
Content-Type: application/json
Content-length: 202

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
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
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "27221b5b-1b5b-2722-5b1b-22275b1b2227",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```

