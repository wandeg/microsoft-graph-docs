---
title: "Update azureADFeatureUsage"
description: "Update the properties of a azureADFeatureUsage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update azureADFeatureUsage

Update the properties of a [azureADFeatureUsage](../resources/azureadfeatureusage.md) object.

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
PATCH ** Entity URI for microsoft.graph.azureADFeatureUsage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [azureADFeatureUsage](../resources/azureADFeatureUsage.md) object.

The following table shows the properties that are required when you create the [azureADFeatureUsage](../resources/azureadfeatureusage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|snapshotDateTime|DateTimeOffset||
|featureName|String||
|usage|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [azureADFeatureUsage](../resources/azureadfeatureusage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_azureadfeatureusage"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.azureADFeatureUsage not found
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.azureADFeatureUsage",
  "snapshotDateTime": "2016-12-31T23:56:55.0631898+03:00",
  "featureName": "Feature Name value",
  "usage": 5
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
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.azureADFeatureUsage",
  "id": "621fad09-ad09-621f-09ad-1f6209ad1f62",
  "snapshotDateTime": "2016-12-31T23:56:55.0631898+03:00",
  "featureName": "Feature Name value",
  "usage": 5
}
```

