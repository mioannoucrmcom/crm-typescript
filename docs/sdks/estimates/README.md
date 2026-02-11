# Estimates

## Overview

Estimates

### Available Operations

* [comCrmEstimateSelfServiceResourceEstimateInvoicing](#comcrmestimateselfserviceresourceestimateinvoicing) - Invoicing
* [comCrmEstimateOrderSelfServiceResourceEstimateOrder](#comcrmestimateorderselfserviceresourceestimateorder) - Order Preview

## comCrmEstimateSelfServiceResourceEstimateInvoicing

Returns an estimation of how much a customer will pay when purchasing a product. The estimation includes not just the product’s final price, but also various detailed amounts on how the estimated cost is calculated

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateSelfServiceResource_estimateInvoicing" method="post" path="/self-service/v2/estimates/invoicing" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.estimates.comCrmEstimateSelfServiceResourceEstimateInvoicing({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    accountId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
    lineItems: [
      {
        productId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
        price: 9.99,
        discountValue: 1,
        discountOption: "PERCENTAGE",
        taxModel: "TAX_EXCLUSIVE",
        bundleProductId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
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
import { estimatesComCrmEstimateSelfServiceResourceEstimateInvoicing } from "crm/funcs/estimates-com-crm-estimate-self-service-resource-estimate-invoicing.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await estimatesComCrmEstimateSelfServiceResourceEstimateInvoicing(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    accountId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
    lineItems: [
      {
        productId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
        price: 9.99,
        discountValue: 1,
        discountOption: "PERCENTAGE",
        taxModel: "TAX_EXCLUSIVE",
        bundleProductId: "be091e01-1842-4a2a-a1ae-e7c2f5343867",
      },
    ],
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("estimatesComCrmEstimateSelfServiceResourceEstimateInvoicing failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingRequest](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-request.md)           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingSecurity](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-security.md)         | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingResponse](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmEstimateOrderSelfServiceResourceEstimateOrder

Preview order information before making an order including fulfillment and invoice estimations
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

<!-- UsageSnippet language="typescript" operationID="com.crm.EstimateOrderSelfServiceResource_estimateOrder" method="post" path="/self-service/v2/estimates/orders" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.estimates.comCrmEstimateOrderSelfServiceResourceEstimateOrder({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    accountId: "1bd3e4d3-5981-209b-787d-352dcd5389a3",
    supplyMethod: "PICK_UP",
    deliveryMethod: "COURIER_SERVICE",
    fulfilledBy: "",
    requestedDeliveryAt: {
      time: 30,
      timeUnit: "MINUTE",
      date: 12312323123,
    },
    addressId: "84bfd840-b520-5bde-8f0a-b36937a2fce7",
    notes: "Sample Notes",
    walletFundsAmount: 1,
    paymentMethodType: "CASH",
    pass: {
      code: "TB68937255",
      pin: "",
    },
    preferredBillingDay: {
      dayOfWeek: "MONDAY",
      dayOfMonth: 1,
      monthOfYear: "JANUARY",
    },
    items: [
      {
        id: "7f45ad8a-b164-2a67-eb93-8651c0f1b101",
        quantity: 1,
        price: 2.99,
        priceTermsId: "905a4a5d-80d4-1e18-4595-d03c2b9546e1",
        components: [
          {
            id: "6e111025-002b-48d7-a675-6d9e48070b8f",
            quantity: 1,
            price: 0.5,
            taxModel: "TAX_INCLUSIVE",
            priceTermsId: "Applicable only when ordering a service bundle",
          },
        ],
      },
    ],
    currentLocation: {
      addressLine1: "17 Baker Str",
      addressLine2: "",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "12462",
      countryCode: "GRC",
      lat: 12.345,
      lon: 11.452,
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
import { estimatesComCrmEstimateOrderSelfServiceResourceEstimateOrder } from "crm/funcs/estimates-com-crm-estimate-order-self-service-resource-estimate-order.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await estimatesComCrmEstimateOrderSelfServiceResourceEstimateOrder(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    accountId: "1bd3e4d3-5981-209b-787d-352dcd5389a3",
    supplyMethod: "PICK_UP",
    deliveryMethod: "COURIER_SERVICE",
    fulfilledBy: "",
    requestedDeliveryAt: {
      time: 30,
      timeUnit: "MINUTE",
      date: 12312323123,
    },
    addressId: "84bfd840-b520-5bde-8f0a-b36937a2fce7",
    notes: "Sample Notes",
    walletFundsAmount: 1,
    paymentMethodType: "CASH",
    pass: {
      code: "TB68937255",
      pin: "",
    },
    preferredBillingDay: {
      dayOfWeek: "MONDAY",
      dayOfMonth: 1,
      monthOfYear: "JANUARY",
    },
    items: [
      {
        id: "7f45ad8a-b164-2a67-eb93-8651c0f1b101",
        quantity: 1,
        price: 2.99,
        priceTermsId: "905a4a5d-80d4-1e18-4595-d03c2b9546e1",
        components: [
          {
            id: "6e111025-002b-48d7-a675-6d9e48070b8f",
            quantity: 1,
            price: 0.5,
            taxModel: "TAX_INCLUSIVE",
            priceTermsId: "Applicable only when ordering a service bundle",
          },
        ],
      },
    ],
    currentLocation: {
      addressLine1: "17 Baker Str",
      addressLine2: "",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "12462",
      countryCode: "GRC",
      lat: 12.345,
      lon: 11.452,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("estimatesComCrmEstimateOrderSelfServiceResourceEstimateOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderRequest](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderSecurity](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-security.md)      | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderResponse](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |