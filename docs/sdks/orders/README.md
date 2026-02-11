# Orders

## Overview

Group containing Orders Web APIs

### Available Operations

* [comCrmOrderSelfServiceResourceListOrders](#comcrmorderselfserviceresourcelistorders) - List Orders
* [comCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder](#comcrmestimateorderfulfillmentselfserviceresourceestimateorder) - Order Fulfillment
* [comCrmOrderSelfServiceResourceCreateOrder](#comcrmorderselfserviceresourcecreateorder) - Submit Order
* [comCrmOrderSelfServiceResourceGetOrder](#comcrmorderselfserviceresourcegetorder) - Get Order
* [comCrmOrderSelfServiceResourcePerformOrderActions](#comcrmorderselfserviceresourceperformorderactions) - Perform Order Actions

## comCrmOrderSelfServiceResourceListOrders

Retrieves a list of a contact’s Orders

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_listOrders" method="get" path="/self-service/v2/contacts/{id}/orders" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceListOrders({
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
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
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceListOrders } from "crm/funcs/orders-com-crm-order-self-service-resource-list-orders.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceListOrders(crm, {
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceListOrders failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_listOrders" method="get" path="/self-service/v2/contacts/{id}/orders" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceListOrders({
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
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
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceListOrders } from "crm/funcs/orders-com-crm-order-self-service-resource-list-orders.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceListOrders(crm, {
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceListOrders failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_listOrders" method="get" path="/self-service/v2/contacts/{id}/orders" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceListOrders({
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
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
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceListOrders } from "crm/funcs/orders-com-crm-order-self-service-resource-list-orders.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceListOrders(crm, {
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceListOrders failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_listOrders" method="get" path="/self-service/v2/contacts/{id}/orders" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceListOrders({
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
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
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceListOrders } from "crm/funcs/orders-com-crm-order-self-service-resource-list-orders.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceListOrders(crm, {
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceListOrders failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_listOrders" method="get" path="/self-service/v2/contacts/{id}/orders" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceListOrders({
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
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
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceListOrders } from "crm/funcs/orders-com-crm-order-self-service-resource-list-orders.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceListOrders(crm, {
    id: "067083a5-607c-959e-e62a-3ba8d359bdd6",
    customFields: "key;value;key;value",
    includeCustomFields: true,
    state: "NEW",
    supplyMethod: "DELIVERY",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceListOrders failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceListOrdersRequest](../../models/operations/com-crm-order-self-service-resource-list-orders-request.md)                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderSelfServiceResourceListOrdersResponse](../../models/operations/com-crm-order-self-service-resource-list-orders-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder

Preview order fulfillment information
                                    <h4>Notes</h4>
                                    <div><div><div><strong>ORDER FLOW</strong></div><p>Integrating an order flow the following APIs should be called
The following APIs should be called in order to make an order</p>
<ol>
<li>Order Fulfillment</li>
<li>Orders Preview</li>
<li>Submit Order</li>
</ol>
</div>
</div>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateOrderFulfillmentSelfServiceResource_estimateOrder" method="post" path="/self-service/v2/estimates/order_fulfillment" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder({
    supplyMethod: "DIRECT_SALE",
    postalCode: "2415",
    latLot: "35.157204,33.314151",
    addressId: "28441e3e-767a-b6cc-9a59-6d7705de6428",
    requestedDeliveryAt: {
      time: 30,
      timeUnit: "MINUTE",
      date: 12312323123,
    },
    isOpen: true,
    requestedOrganisationId: "4456e728-019c-86e4-3e4f-bb7920e2ef75",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { ordersComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder } from "crm/funcs/orders-com-crm-estimate-order-fulfillment-self-service-resource-estimate-order.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder(crm, {
    supplyMethod: "DIRECT_SALE",
    postalCode: "2415",
    latLot: "35.157204,33.314151",
    addressId: "28441e3e-767a-b6cc-9a59-6d7705de6428",
    requestedDeliveryAt: {
      time: 30,
      timeUnit: "MINUTE",
      date: 12312323123,
    },
    isOpen: true,
    requestedOrganisationId: "4456e728-019c-86e4-3e4f-bb7920e2ef75",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                      | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                      | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderRequest](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-request.md) | :heavy_check_mark:                                                                                                                                                                             | The request object to use for the request.                                                                                                                                                     |
| `options`                                                                                                                                                                                      | RequestOptions                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                        | :heavy_minus_sign:                                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                 |
| `options.retries`                                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                                               |

### Response

**Promise\<[operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderResponse](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrderSelfServiceResourceCreateOrder

Creates a new Order for a contact based on an order’s estimation
                                    <h4>Notes</h4>
                                    <div><div><div><strong>ORDER FLOW</strong></div><p>Integrating an order flow the following APIs should be called
The following APIs should be called in order to make an order</p>
<ol>
<li>Order Fulfillment</li>
<li>Orders Preview</li>
<li>Submit Order</li>
</ol>
</div>
</div>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_createOrder" method="post" path="/self-service/v2/orders" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceCreateOrder({
    estimationId: "37b56acf-665c-1112-93fc-163b3639bcbe",
    useWalletFunds: true,
    walletFundsAmount: 11.99,
    notes: "Lorem Ipsum",
    useAccountFunds: true,
    payments: [
      {
        paymentMethodType: "CRM_WALLET",
        paidOn: "ON_ORDER",
        paymentMethodId: "37b56acf-665c-1112-93fc-163b3639bcbe",
        amount: 112.12,
      },
    ],
    customFields: [
      {
        key: "custom_key",
        value: "0001-345",
      },
    ],
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceCreateOrder } from "crm/funcs/orders-com-crm-order-self-service-resource-create-order.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceCreateOrder(crm, {
    estimationId: "37b56acf-665c-1112-93fc-163b3639bcbe",
    useWalletFunds: true,
    walletFundsAmount: 11.99,
    notes: "Lorem Ipsum",
    useAccountFunds: true,
    payments: [
      {
        paymentMethodType: "CRM_WALLET",
        paidOn: "ON_ORDER",
        paymentMethodId: "37b56acf-665c-1112-93fc-163b3639bcbe",
        amount: 112.12,
      },
    ],
    customFields: [
      {
        key: "custom_key",
        value: "0001-345",
      },
    ],
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceCreateOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceCreateOrderRequest](../../models/operations/com-crm-order-self-service-resource-create-order-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderSelfServiceResourceCreateOrderResponse](../../models/operations/com-crm-order-self-service-resource-create-order-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrderSelfServiceResourceGetOrder

Retrieves detailed information for a specific order

### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_getOrder" method="get" path="/self-service/v2/orders/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceGetOrder({
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceGetOrder } from "crm/funcs/orders-com-crm-order-self-service-resource-get-order.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceGetOrder(crm, {
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceGetOrder failed:", res.error);
  }
}

run();
```
### Example Usage: Example 2

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_getOrder" method="get" path="/self-service/v2/orders/{id}" example="Example 2" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourceGetOrder({
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { ordersComCrmOrderSelfServiceResourceGetOrder } from "crm/funcs/orders-com-crm-order-self-service-resource-get-order.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourceGetOrder(crm, {
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourceGetOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceGetOrderRequest](../../models/operations/com-crm-order-self-service-resource-get-order-request.md)                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderSelfServiceResourceGetOrderResponse](../../models/operations/com-crm-order-self-service-resource-get-order-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmOrderSelfServiceResourcePerformOrderActions

Updates an existing Order

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.OrderSelfServiceResource_performOrderActions" method="put" path="/self-service/v2/orders/{id}/actions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.orders.comCrmOrderSelfServiceResourcePerformOrderActions({
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
    body: {
      action: "CANCEL",
      cancellationReasonId: "553f91e9-a418-354e-1e69-4b6dac24558e",
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
import { ordersComCrmOrderSelfServiceResourcePerformOrderActions } from "crm/funcs/orders-com-crm-order-self-service-resource-perform-order-actions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await ordersComCrmOrderSelfServiceResourcePerformOrderActions(crm, {
    id: "6514df04-9218-d354-9d59-ed9e98882fe6",
    body: {
      action: "CANCEL",
      cancellationReasonId: "553f91e9-a418-354e-1e69-4b6dac24558e",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("ordersComCrmOrderSelfServiceResourcePerformOrderActions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourcePerformOrderActionsRequest](../../models/operations/com-crm-order-self-service-resource-perform-order-actions-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmOrderSelfServiceResourcePerformOrderActionsResponse](../../models/operations/com-crm-order-self-service-resource-perform-order-actions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |