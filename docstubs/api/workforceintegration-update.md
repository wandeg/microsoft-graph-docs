---
title: "Update workforceIntegration"
description: "Update the properties of a workforceIntegration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workforceIntegration

Namespace: microsoft.graph

Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.

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
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workforceIntegration](../resources/workforceintegration.md) object.

The following table shows the properties that are required when you create the [workforceIntegration](../resources/workforceintegration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String||
|apiVersion|Int32||
|encryption|[workforceIntegrationEncryption](../resources/workforceintegrationencryption.md)||
|isActive|Boolean||
|url|String||
|supports|Enumeration| Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|supportedEntities|Enumeration| Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "displayName": "Display Name value",
  "apiVersion": 10,
  "encryption": {
    "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
    "protocol": "String",
    "secret": "Secret value"
  },
  "isActive": true,
  "url": "Url value",
  "supports": "String",
  "supportedEntities": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 923

{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "id": "4c41d897-d897-4c41-97d8-414c97d8414c",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "displayName": "Display Name value",
  "apiVersion": 10,
  "encryption": {
    "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
    "protocol": "String",
    "secret": "Secret value"
  },
  "isActive": true,
  "url": "Url value",
  "supports": "String",
  "supportedEntities": "String"
}
```

