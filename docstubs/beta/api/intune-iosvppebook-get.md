---
title: "Get iosVppEBook"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get iosVppEBook

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships an iosVppEBook object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request Body

<!-- Actions and Functions -->

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an iosVppEBook object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_iosvppebook"
}
-->

```http
GET https://graph.microsoft.com/beta

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.iosVppEBook"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "appleId": "String",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "genres": [
    "String"
  ],
  "id": "String(identifier)",
  "informationUrl": "String",
  "language": "String",
  "largeCover": {
    "@odata.type": "#microsoft.graph.mimeContent",
    "type": "String",
    "value": "Binary"
  },
  "lastModifiedDateTime": "DateTimeOffset",
  "privacyInformationUrl": "String",
  "publishedDateTime": "DateTimeOffset",
  "publisher": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "seller": "String",
  "totalLicenseCount": "Int32",
  "usedLicenseCount": "Int32",
  "vppOrganizationName": "String",
  "vppTokenId": "Guid"
}
}

```