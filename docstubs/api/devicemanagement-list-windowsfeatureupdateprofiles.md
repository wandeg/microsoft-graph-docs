---
title: "List windowsFeatureUpdateProfiles"
description: "Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsFeatureUpdateProfiles

Namespace: microsoft.graph

Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property.

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
GET /deviceManagement/windowsFeatureUpdateProfiles
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsfeatureupdateprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsfeatureupdateprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
      "id": "2b8932be-32be-2b89-be32-892bbe32892b",
      "displayName": "Display Name value",
      "description": "Description value",
      "featureUpdateVersion": "Feature Update Version value",
      "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
    }
  ]
}
```

