---
title: "Create userExperienceAnalyticsScoreHistory"
description: "Create a new userExperienceAnalyticsScoreHistory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsScoreHistory

Namespace: microsoft.graph

Create a new userExperienceAnalyticsScoreHistory object.

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
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics device startup process.|
|startupDateTime|DateTimeOffset|The user experience analytics device startup date time.|
|startupScore|Int32|User experience analytics device startup score.|
|coreBootScore|Int32|The user experience analytics device core boot score.|
|coreSigninScore|Int32|The User experience analytics device core sign-in score.|
|recommendedSoftwareScore|Int32|The User experience analytics device core sign-in score.|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsscorehistory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-Type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "String (timestamp)",
  "startupScore": "Integer",
  "coreBootScore": "Integer",
  "coreSigninScore": "Integer",
  "recommendedSoftwareScore": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userexperienceanalyticsscorehistory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsScoreHistory",
  "id": "abc55b47-5b47-abc5-475b-c5ab475bc5ab",
  "startupDateTime": "String (timestamp)",
  "startupScore": "Integer",
  "coreBootScore": "Integer",
  "coreSigninScore": "Integer",
  "recommendedSoftwareScore": "Integer"
}
```

