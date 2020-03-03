---
title: "Add workforceIntegrations"
description: "Add workforceIntegrations by posting to the workforceIntegrations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add workforceIntegrations

Namespace: microsoft.graph

Add workforceIntegrations by posting to the workforceIntegrations collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teamwork/workforceIntegrations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
|supports|Enumeration|. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/teamwork/workforceIntegrations
Content-type: application/json
Content-length: 344

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
  "supports": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceintegration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 888

{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "id": "2a6dc170-c170-2a6d-70c1-6d2a70c16d2a",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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
  "supports": "String"
}
```

