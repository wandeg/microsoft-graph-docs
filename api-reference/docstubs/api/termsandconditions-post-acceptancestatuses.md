---
title: "Create acceptanceStatuses"
description: "Create a new acceptanceStatuses object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create acceptanceStatuses

Namespace: microsoft.graph

Create a new acceptanceStatuses object.

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
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.

The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|Display name of the user whose acceptance the entity represents.|
|acceptedVersion|Int32|Most recent version number of the T&C accepted by the user.|
|acceptedDateTime|DateTimeOffset|DateTime when the terms were last accepted by the user.|



## Response
If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_termsandconditionsacceptancestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2017-01-01T00:02:45.3533816+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termsandconditionsacceptancestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "72de1fee-1fee-72de-ee1f-de72ee1fde72",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2017-01-01T00:02:45.3533816+03:00"
}
```

