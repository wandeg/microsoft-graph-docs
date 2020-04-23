---
title: "Update columns"
description: "Update the properties of a columns object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update columns

Namespace: microsoft.graph

Update the properties of a columns object.

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
PATCH /invitations/{invitationsId}/invitedUser/drive/list/columns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [columnDefinition](../resources/columndefinition.md) object.

The following table shows the properties that are required when you create the [columnDefinition](../resources/columndefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|boolean|[booleanColumn](../resources/booleancolumn.md)|**TODO: Add Description**|
|calculated|[calculatedColumn](../resources/calculatedcolumn.md)|**TODO: Add Description**|
|choice|[choiceColumn](../resources/choicecolumn.md)|**TODO: Add Description**|
|columnGroup|String|**TODO: Add Description**|
|currency|[currencyColumn](../resources/currencycolumn.md)|**TODO: Add Description**|
|dateTime|[dateTimeColumn](../resources/datetimecolumn.md)|**TODO: Add Description**|
|defaultValue|[defaultColumnValue](../resources/defaultcolumnvalue.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enforceUniqueValues|Boolean|**TODO: Add Description**|
|hidden|Boolean|**TODO: Add Description**|
|indexed|Boolean|**TODO: Add Description**|
|lookup|[lookupColumn](../resources/lookupcolumn.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|number|[numberColumn](../resources/numbercolumn.md)|**TODO: Add Description**|
|personOrGroup|[personOrGroupColumn](../resources/personorgroupcolumn.md)|**TODO: Add Description**|
|readOnly|Boolean|**TODO: Add Description**|
|required|Boolean|**TODO: Add Description**|
|text|[textColumn](../resources/textcolumn.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [columnDefinition](../resources/columndefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_columns"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/list/columns
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "id": "a4330f66-0f66-a433-660f-33a4660f33a4",
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

