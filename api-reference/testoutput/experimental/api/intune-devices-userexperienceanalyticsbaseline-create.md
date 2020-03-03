---
title: "Create userExperienceAnalyticsBaseline"
description: "Create a new userExperienceAnalyticsBaseline object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create userExperienceAnalyticsBaseline

Namespace: microsoft.graph

Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.

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
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name of the user experience analytics baseline.|
|isBuiltIn|Boolean|Signifies if the current baseline is the commercial median baseline or a custom baseline.|
|createdDateTime|DateTimeOffset|The date the custom baseline was created.|



## Response
If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsbaseline_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "isBuiltIn": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsbaseline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "404d41c1-41c1-404d-c141-4d40c1414d40",
  "displayName": "Display Name value",
  "isBuiltIn": true,
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00"
}
```

