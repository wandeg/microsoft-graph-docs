---
title: "Add columns"
description: "Add columns by posting to the columns collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add columns

Add columns by posting to the columns collection.

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
POST /sites/{sitesId}/columns/$ref
POST /me/joinedTeams/{groupId}/sites/{siteId}/columns/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the columnDefinition object.

The following table shows the properties that are required when you create the columnDefinition.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|boolean|[booleanColumn](../resources/booleanColumn.md)||
|calculated|[calculatedColumn](../resources/calculatedColumn.md)||
|choice|[choiceColumn](../resources/choiceColumn.md)||
|columnGroup|String||
|currency|[currencyColumn](../resources/currencyColumn.md)||
|dateTime|[dateTimeColumn](../resources/dateTimeColumn.md)||
|defaultValue|[defaultColumnValue](../resources/defaultColumnValue.md)||
|description|String||
|displayName|String||
|enforceUniqueValues|Boolean||
|hidden|Boolean||
|indexed|Boolean||
|lookup|[lookupColumn](../resources/lookupColumn.md)||
|name|String||
|number|[numberColumn](../resources/numberColumn.md)||
|personOrGroup|[personOrGroupColumn](../resources/personOrGroupColumn.md)||
|readOnly|Boolean||
|required|Boolean||
|text|[textColumn](../resources/textColumn.md)||



## Response
If successful, this method returns a `201 Created` response code and a [columnDefinition](../resources/columndefinition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_columndefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/sites/{sitesId}/columns
Content-type: application/json
Content-length: 1904

{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn",
    "format": "Format value",
    "formula": "Formula value",
    "outputType": "Output Type value"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn",
    "allowTextEntry": true,
    "choices": [
      "Choices value"
    ],
    "displayAs": "Display As value"
  },
  "columnGroup": "Column Group value",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn",
    "locale": "Locale value"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue",
    "value": "Value value"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "enforceUniqueValues": true,
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn",
    "allowMultipleValues": true,
    "allowUnlimitedLength": true,
    "columnName": "Column Name value",
    "listId": "List Id value",
    "primaryLookupColumnId": "Primary Lookup Column Id value"
  },
  "name": "Name value",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn",
    "decimalPlaces": "Decimal Places value",
    "maximum": "Double",
    "minimum": "Double"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn",
    "allowMultipleSelection": true,
    "chooseFromType": "Choose From Type value"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn",
    "allowMultipleLines": true,
    "appendChangesToExistingText": true,
    "linesForEditing": 15,
    "maxLength": 9,
    "textType": "Text Type value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columndefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1953

{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "id": "89105bca-5bca-8910-ca5b-1089ca5b1089",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn",
    "format": "Format value",
    "formula": "Formula value",
    "outputType": "Output Type value"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn",
    "allowTextEntry": true,
    "choices": [
      "Choices value"
    ],
    "displayAs": "Display As value"
  },
  "columnGroup": "Column Group value",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn",
    "locale": "Locale value"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue",
    "value": "Value value"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "enforceUniqueValues": true,
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn",
    "allowMultipleValues": true,
    "allowUnlimitedLength": true,
    "columnName": "Column Name value",
    "listId": "List Id value",
    "primaryLookupColumnId": "Primary Lookup Column Id value"
  },
  "name": "Name value",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn",
    "decimalPlaces": "Decimal Places value",
    "maximum": "Double",
    "minimum": "Double"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn",
    "allowMultipleSelection": true,
    "chooseFromType": "Choose From Type value"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn",
    "allowMultipleLines": true,
    "appendChangesToExistingText": true,
    "linesForEditing": 15,
    "maxLength": 9,
    "textType": "Text Type value"
  }
}
```

