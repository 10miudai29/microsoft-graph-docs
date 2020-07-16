---
title: "Get tasks"
description: "Read the properties and relationships of a Task object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get tasks
Namespace: microsoft.graph

Read the properties and relationships of a [Task](../resources/task.md) object.

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
GET /lists/{listsId}/tasks
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [Task](../resources/task.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_task"
}
-->
``` http
GET https://graph.microsoft.com/beta/lists/{listsId}/tasks
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Task"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.Task",
    "id": "91b682f7-82f7-91b6-f782-b691f782b691",
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "importance": "String",
    "isReminderOn": "Boolean",
    "recurrence": {
      "@odata.type": "microsoft.graph.patternedRecurrence"
    },
    "reminderDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "status": "String",
    "title": "String",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "bodyLastModifiedDateTime": "String (timestamp)"
  }
}
```

