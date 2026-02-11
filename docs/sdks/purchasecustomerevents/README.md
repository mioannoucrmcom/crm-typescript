# PurchaseCustomerEvents

## Overview

Purchase Customer Events

### Available Operations

* [comCrmPurchaseCustomerEventSelfServiceResourceListPurchases](#comcrmpurchasecustomereventselfserviceresourcelistpurchases) - Search Contact Purchases
* [comCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase](#comcrmpurchasecustomereventselfserviceresourcereclaimpurchase) - Reclaim Purchase To Contact
* [comCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase](#comcrmpurchasecustomereventselfserviceresourcegetsinglepurchase) - Get Purchase
* [comCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions](#comcrmpurchasecustomereventselfserviceresourcegetpurchaserewardtransactions) - List Purchase Rewards Breakdown

## comCrmPurchaseCustomerEventSelfServiceResourceListPurchases

Retrieve a list of contact's purchase events based on search criteria (e.g. all purchases)

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_listPurchases" method="get" path="/self-service/v2/contacts/{id}/purchases" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceListPurchases({
    id: "<id>",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-list-purchases.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_listPurchases" method="get" path="/self-service/v2/contacts/{id}/purchases" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceListPurchases({
    id: "<id>",
    includeTotal: true,
    size: 100,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-list-purchases.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_listPurchases" method="get" path="/self-service/v2/contacts/{id}/purchases" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceListPurchases({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-list-purchases.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_listPurchases" method="get" path="/self-service/v2/contacts/{id}/purchases" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceListPurchases({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-list-purchases.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_listPurchases" method="get" path="/self-service/v2/contacts/{id}/purchases" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceListPurchases({
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-list-purchases.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases(crmcom, {
    id: "<id>",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceListPurchases failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                | Type                                                                                                                                                                                     | Required                                                                                                                                                                                 | Description                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesRequest](../../models/operations/com-crm-purchase-customer-event-self-service-resource-list-purchases-request.md) | :heavy_check_mark:                                                                                                                                                                       | The request object to use for the request.                                                                                                                                               |
| `options`                                                                                                                                                                                | RequestOptions                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                       | Used to set various options for making HTTP requests.                                                                                                                                    |
| `options.fetchOptions`                                                                                                                                                                   | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                  | :heavy_minus_sign:                                                                                                                                                                       | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.           |
| `options.retries`                                                                                                                                                                        | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                       | Enables retrying HTTP requests under certain failure conditions.                                                                                                                         |

### Response

**Promise\<[operations.ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesResponse](../../models/operations/com-crm-purchase-customer-event-self-service-resource-list-purchases-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase

Reclaim a purchase customer event to a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_reclaimPurchase" method="post" path="/self-service/v2/purchases/reclaim" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase({
    id: "sdfsdfsdf4-43-r-few-f-wf-r3443;1234",
    organisation: {
      merchantTap: {
        code: "MT001",
      },
      venueTap: {
        code: "VT001",
      },
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-reclaim-purchase.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase(crmcom, {
    id: "sdfsdfsdf4-43-r-few-f-wf-r3443;1234",
    organisation: {
      merchantTap: {
        code: "MT001",
      },
      venueTap: {
        code: "VT001",
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchase failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                    | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                    | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseRequest](../../models/operations/com-crm-purchase-customer-event-self-service-resource-reclaim-purchase-request.md) | :heavy_check_mark:                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                   |
| `options`                                                                                                                                                                                    | RequestOptions                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                      | :heavy_minus_sign:                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.               |
| `options.retries`                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                             |

### Response

**Promise\<[operations.ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseResponse](../../models/operations/com-crm-purchase-customer-event-self-service-resource-reclaim-purchase-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase

Retrieve detailed information for a purchase event

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_getSinglePurchase" method="get" path="/self-service/v2/purchases/{id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase({
    id: "a0003f83-32c8-da03-200d-d6af0386cb3a",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-get-single-purchase.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase(crmcom, {
    id: "a0003f83-32c8-da03-200d-d6af0386cb3a",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchase failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                         | Type                                                                                                                                                                                              | Required                                                                                                                                                                                          | Description                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                         | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseRequest](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-single-purchase-request.md) | :heavy_check_mark:                                                                                                                                                                                | The request object to use for the request.                                                                                                                                                        |
| `options`                                                                                                                                                                                         | RequestOptions                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                | Used to set various options for making HTTP requests.                                                                                                                                             |
| `options.fetchOptions`                                                                                                                                                                            | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                    |
| `options.retries`                                                                                                                                                                                 | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                  |

### Response

**Promise\<[operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseResponse](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-single-purchase-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions

Get reward details for a specific purchase customer event

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PurchaseCustomerEventSelfServiceResource_getPurchaseRewardTransactions" method="get" path="/self-service/v2/purchases/{id}/rewards" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.purchaseCustomerEvents.comCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions({
    authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
  }, {
    id: "cd953fe3-e2f6-2ae2-8a40-1bd8154c0f29",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import {
  purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions,
} from "crmcom/funcs/purchase-customer-events-com-crm-purchase-customer-event-self-service-resource-get-purchase-reward-transactions.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions(crmcom, {
    authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
  }, {
    id: "cd953fe3-e2f6-2ae2-8a40-1bd8154c0f29",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("purchaseCustomerEventsComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                                                    | Type                                                                                                                                                                                                                         | Required                                                                                                                                                                                                                     | Description                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                                                    | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsRequest](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-purchase-reward-transactions-request.md)   | :heavy_check_mark:                                                                                                                                                                                                           | The request object to use for the request.                                                                                                                                                                                   |
| `security`                                                                                                                                                                                                                   | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsSecurity](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-purchase-reward-transactions-security.md) | :heavy_check_mark:                                                                                                                                                                                                           | The security requirements to use for the request.                                                                                                                                                                            |
| `options`                                                                                                                                                                                                                    | RequestOptions                                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                                           | Used to set various options for making HTTP requests.                                                                                                                                                                        |
| `options.fetchOptions`                                                                                                                                                                                                       | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                                                           | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                                               |
| `options.retries`                                                                                                                                                                                                            | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                                                           | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                                             |

### Response

**Promise\<[operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsResponse](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-purchase-reward-transactions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |