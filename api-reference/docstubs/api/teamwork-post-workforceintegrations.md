---
title: "Create workforceIntegrations"
description: "Create a new workforceIntegrations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create workforceIntegrations

Namespace: microsoft.graph

Create a new workforceIntegrations object.

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
POST /teamwork/workforceIntegrations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workforceIntegration](../resources/workforceintegration.md) object.

The following table shows the properties that are required when you create the [workforceIntegration](../resources/workforceintegration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String|**TODO: Add Description**|
|apiVersion|Int32|**TODO: Add Description**|
|encryption|[workforceIntegrationEncryption](../resources/workforceintegrationencryption.md)|**TODO: Add Description**|
|isActive|Boolean|**TODO: Add Description**|
|url|String|**TODO: Add Description**|
|supports|workforceIntegrationSupportedEntities|**TODO: Add Description**. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|supportedEntities|workforceIntegrationSupportedEntities|**TODO: Add Description**. Possible values are: `none`, `shift`, `swapRequest`, `userShiftPreferences`, `openShift`, `openShiftRequest`, `offerShiftRequest`, `unknownFutureValue`.|
|eligibilityFilteringEnabledEntities|eligibilityFilteringEnabledEntities|**TODO: Add Description**. Possible values are: `none`, `swapRequest`, `offerShiftRequest`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-Type: application/json
Content-length: 430

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
  "supportedEntities": "String",
  "eligibilityFilteringEnabledEntities": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceintegration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workforceIntegration",
  "id": "2203230c-230c-2203-0c23-03220c230322",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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
  "supportedEntities": "String",
  "eligibilityFilteringEnabledEntities": "String"
}
```

