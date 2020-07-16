---
title: "Update lists"
description: "Update the properties of a lists object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update lists
Namespace: microsoft.graph

Update the properties of a lists object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

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
PATCH /todo/lists
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [TaskList](../resources/tasklist.md) object.

The following table shows the properties that are required when you create the [TaskList](../resources/tasklist.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|isOwner|Boolean|**TODO: Add Description**|
|isShared|Boolean|**TODO: Add Description**|
|wellknownListName|wellknownListName|**TODO: Add Description**. Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [TaskList](../resources/tasklist.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_lists"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/todo/lists
Content-Type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.TaskList",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
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
  "@odata.type": "#microsoft.graph.TaskList",
  "id": "61f1a6b5-a6b5-61f1-b5a6-f161b5a6f161",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

