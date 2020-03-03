---
title: "Update workforceIntegration"
description: "Update the properties of a workforceIntegration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workforceIntegration

Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.

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
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workforceIntegration](../resources/workforceIntegration.md) object.

The following table shows the properties that are required when you create the [workforceIntegration](../resources/workforceintegration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|displayName|String||
|apiVersion|Int32||
|encryption|[workforceIntegrationEncryption](../resources/workforceIntegrationEncryption.md)||
|isActive|Boolean||
|url|String||
|supports|Enumeration|. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/teamwork/workforceIntegrations/{workforceIntegrationId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "id": "0ce9b8e3-b8e3-0ce9-e3b8-e90ce3b8e90c",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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

