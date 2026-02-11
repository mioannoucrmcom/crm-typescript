# CommercePools

## Overview

Commerce Pools

### Available Operations

* [comCrmCommercePoolSelfServiceResourceActions](#comcrmcommercepoolselfserviceresourceactions) - Commerce Pool Actions

## comCrmCommercePoolSelfServiceResourceActions

Perform actions on existing commerce pool (e.g. activate commerce pool)

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.CommercePoolSelfServiceResource_actions" method="put" path="/self-service/v2/commerce_pools/{id}/actions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.commercePools.comCrmCommercePoolSelfServiceResourceActions({
    id: "c0d4712e-6688-4604-b3d6-d084e4d2dc05",
    body: {
      action: "ACTIVATE",
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
import { commercePoolsComCrmCommercePoolSelfServiceResourceActions } from "crm/funcs/commerce-pools-com-crm-commerce-pool-self-service-resource-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await commercePoolsComCrmCommercePoolSelfServiceResourceActions(crm, {
    id: "c0d4712e-6688-4604-b3d6-d084e4d2dc05",
    body: {
      action: "ACTIVATE",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("commercePoolsComCrmCommercePoolSelfServiceResourceActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmCommercePoolSelfServiceResourceActionsRequest](../../models/operations/com-crm-commerce-pool-self-service-resource-actions-request.md)                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmCommercePoolSelfServiceResourceActionsResponse](../../models/operations/com-crm-commerce-pool-self-service-resource-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |