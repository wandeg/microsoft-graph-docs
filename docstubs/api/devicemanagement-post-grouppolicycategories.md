---
title: "Add groupPolicyCategories"
description: "Add groupPolicyCategories by posting to the groupPolicyCategories collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add groupPolicyCategories

Namespace: microsoft.graph

Add groupPolicyCategories by posting to the groupPolicyCategories collection.

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
POST /deviceManagement/groupPolicyCategories/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/grouppolicycategory.md) object.

The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/grouppolicycategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|isRoot|Boolean||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [groupPolicyCategory](../resources/grouppolicycategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouppolicycategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicycategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "id": "42a52978-2978-42a5-7829-a5427829a542",
  "displayName": "Display Name value",
  "isRoot": true,
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

