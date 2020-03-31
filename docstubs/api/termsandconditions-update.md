---
title: "Update termsAndConditions"
description: "Update the properties of a termsAndConditions object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update termsAndConditions

Namespace: microsoft.graph

Update the properties of a [termsAndConditions](../resources/termsandconditions.md) object.

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
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [termsAndConditions](../resources/termsandconditions.md) object.

The following table shows the properties that are required when you create the [termsAndConditions](../resources/termsandconditions.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|displayName|String||
|description|String||
|title|String||
|bodyText|String||
|acceptanceStatement|String||
|version|Int32||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/termsandconditions.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_termsandconditions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
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
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "98bac0af-c0af-98ba-afc0-ba98afc0ba98",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "modifiedDateTime": "2017-01-01T00:01:43.3164239+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

