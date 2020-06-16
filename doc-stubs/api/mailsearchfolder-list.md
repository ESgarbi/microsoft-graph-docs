---
title: "List mailSearchFolders"
description: "Get a list of the mailSearchFolder objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mailSearchFolders
Namespace: microsoft.graph

Get a list of the [mailSearchFolder](../resources/mailsearchfolder.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.mailSearchFolder not found
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

If successful, this method returns a `200 OK` response code and a collection of [mailSearchFolder](../resources/mailsearchfolder.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mailsearchfolder"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.mailSearchFolder not found
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailsearchfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "f162a343-a343-f162-43a3-62f143a362f1",
      "displayName": "String",
      "parentFolderId": "String",
      "childFolderCount": "Integer",
      "unreadItemCount": "Integer",
      "totalItemCount": "Integer",
      "wellKnownName": "String",
      "isSupported": "Boolean",
      "includeNestedFolders": "Boolean",
      "sourceFolderIds": [
        "String"
      ],
      "filterQuery": "String"
    }
  ]
}
```

