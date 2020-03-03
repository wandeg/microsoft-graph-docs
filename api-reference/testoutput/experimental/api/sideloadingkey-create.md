---
title: "Create sideLoadingKey"
description: "Create a new sideLoadingKey object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sideLoadingKey

Namespace: microsoft.graph

Create a new [sideLoadingKey](../resources/sideloadingkey.md) object.

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
POST /deviceAppManagement/sideLoadingKeys
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [sideLoadingKey](../resources/sideloadingkey.md) object.

The following table shows the properties that are required when you create the [sideLoadingKey](../resources/sideloadingkey.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String|Side Loading Key Value, it is 5x5 value, seperated by hiphens.|
|displayName|String|Side Loading Key Name displayed to the ITPro Admins.|
|description|String|Side Loading Key description displayed to the ITPro Admins..|
|totalActivation|Int32|Side Loading Key Total Activation displayed to the ITPro Admins.|
|lastUpdatedDateTime|String|Side Loading Key Last Updated Date displayed to the ITPro Admins.|



## Response
If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/sideloadingkey.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sideloadingkey_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sideloadingkey"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "fa969573-9573-fa96-7395-96fa739596fa",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

