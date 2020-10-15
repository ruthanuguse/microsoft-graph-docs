---
title: "List installSummary"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# List installSummary

Namespace: microsoft.graph

Get the eBookInstallSummary objects from an installSummary navigation property.

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

If successful, this method returns a `200 Ok` response code and an eBookInstallSummary object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "list_installsummary"
}
-->

```http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{id}/installSummary

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.eBookInstallSummary"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "failedDeviceCount": "Int32",
  "failedUserCount": "Int32",
  "id": "String(identifier)",
  "installedDeviceCount": "Int32",
  "installedUserCount": "Int32",
  "notInstalledDeviceCount": "Int32",
  "notInstalledUserCount": "Int32"
}
}

```