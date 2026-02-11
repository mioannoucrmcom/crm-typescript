# ContactTokens

## Overview

Contact Tokens

### Available Operations

* [listContactTokensSS](#listcontacttokensss) - List Contact Tokens
* [addContactTokenSS](#addcontacttokenss) - Request Contact Token

## listContactTokensSS

List all contact tokens for a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="listContactTokensSS" method="get" path="/self-service/v2/contacts/{id}/tokens" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactTokens.listContactTokensSS({
    id: "33749faa-4ef0-426d-f9f0-83b91bf5ab3f",
    communityId: "c1d2e3f4-5678-90ab-cdef-1234567890ab",
    intent: "SPEND",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactTokensListContactTokensSS } from "crm/funcs/contact-tokens-list-contact-tokens-ss.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactTokensListContactTokensSS(crm, {
    id: "33749faa-4ef0-426d-f9f0-83b91bf5ab3f",
    communityId: "c1d2e3f4-5678-90ab-cdef-1234567890ab",
    intent: "SPEND",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactTokensListContactTokensSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ListContactTokensSSRequest](../../models/operations/list-contact-tokens-ss-request.md)                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ListContactTokensSSResponse](../../models/operations/list-contact-tokens-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## addContactTokenSS

Request to create a contact token

### Example Usage

<!-- UsageSnippet language="typescript" operationID="addContactTokenSS" method="post" path="/self-service/v2/contacts/{id}/tokens" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactTokens.addContactTokenSS({
    id: "e18ee2bc-c6f3-49e1-8e05-763386378017",
    body: {
      intent: "SPEND",
      spendAmount: 14.52,
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactTokensAddContactTokenSS } from "crm/funcs/contact-tokens-add-contact-token-ss.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactTokensAddContactTokenSS(crm, {
    id: "e18ee2bc-c6f3-49e1-8e05-763386378017",
    body: {
      intent: "SPEND",
      spendAmount: 14.52,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactTokensAddContactTokenSS failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AddContactTokenSSRequest](../../models/operations/add-contact-token-ss-request.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.AddContactTokenSSResponse](../../models/operations/add-contact-token-ss-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |