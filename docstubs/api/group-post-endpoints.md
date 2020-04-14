---
title: "Add endpoints"
description: "Add endpoints by posting to the endpoints collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add endpoints

Namespace: microsoft.graph

Add endpoints by posting to the endpoints collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /groups/{groupsId}/endpoints/$ref
POST /me/joinedGroups/{groupId}/endpoints/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [endpoint](../resources/endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|capability|String||
|providerId|String||
|providerName|String||
|uri|String||
|providerResourceId|String||



## Response
If successful, this method returns a `201 Created` response code and a [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_endpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/endpoints
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "2017-01-01T00:00:54.363956+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "706f9283-9283-706f-8392-6f7083926f70",
  "deletedDateTime": "2017-01-01T00:00:54.363956+03:00",
  "capability": "Capability value",
  "providerId": "Provider Id value",
  "providerName": "Provider Name value",
  "uri": "Uri value",
  "providerResourceId": "Provider Resource Id value"
}
```

