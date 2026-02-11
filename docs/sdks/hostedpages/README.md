# HostedPages

## Overview

Hosted Pages

### Available Operations

* [comCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm](#comcrmhostedpagesselfserviceresourcegenerategiftpasspaymentform) - Get Gift Pass Payment Form
* [comCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm](#comcrmhostedpagesselfserviceresourcegenerateaddpaymentmethodform) - Add Payment Method
* [comCrmHostedPagesSelfServiceResourceGeneratePaymentForm](#comcrmhostedpagesselfserviceresourcegeneratepaymentform) - Payment Form
* [comCrmHostedPagesSelfServiceResourceGeneratePayoutForm](#comcrmhostedpagesselfserviceresourcegeneratepayoutform) - Payout Form

## comCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm

Web API used when consumers purchase Gift Passes from a Landing page. The Web API forwards information of the purchased pass, along with the buyer and receiver's details. In addition, the Web aPI integrates with the Payment Gateway service and request to load their payment form for an easy payment processing. To avoid any issues, it's vital to check the Payment Gateway service's mandatory information requirements, such as the buyer's email, phone, and address information, before triggering the Web API. 

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.HostedPagesSelfServiceResource_generateGiftPassPaymentForm" method="post" path="/self-service/v2/hosted_pages/gift_passes" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.hostedPages.comCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    integrationId: "302fb9b0-d57c-4a07-ae0b-b7cbec934775",
    redirectUrl: "https://myapp.com",
    amount: 9.99,
    currencyCode: "EUR",
    message: "This is a gift",
    passPlanId: "85d5025f-6b6a-4325-b047-a9e85f0a6f07",
    languageCode: "el",
    buyer: {
      name: "John Doe",
      email: "johndoe@crm.com",
      phone: {
        countryCode: "CYP",
        number: "99999999",
      },
      address: {
        addressLine1: "Elia Papakyriakou",
        addressLine2: "Elia Papakyriakou",
        stateProvinceCounty: "Egkomi",
        townCity: "Nicosia",
        postalCode: "2000",
        countryCode: "CYP",
      },
    },
    beneficiary: {
      name: "Jane Doe",
      email: "janedoe@crm.com",
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
import { hostedPagesComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm } from "crm/funcs/hosted-pages-com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await hostedPagesComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    integrationId: "302fb9b0-d57c-4a07-ae0b-b7cbec934775",
    redirectUrl: "https://myapp.com",
    amount: 9.99,
    currencyCode: "EUR",
    message: "This is a gift",
    passPlanId: "85d5025f-6b6a-4325-b047-a9e85f0a6f07",
    languageCode: "el",
    buyer: {
      name: "John Doe",
      email: "johndoe@crm.com",
      phone: {
        countryCode: "CYP",
        number: "99999999",
      },
      address: {
        addressLine1: "Elia Papakyriakou",
        addressLine2: "Elia Papakyriakou",
        stateProvinceCounty: "Egkomi",
        townCity: "Nicosia",
        postalCode: "2000",
        countryCode: "CYP",
      },
    },
    beneficiary: {
      name: "Jane Doe",
      email: "janedoe@crm.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("hostedPagesComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                            | Type                                                                                                                                                                                                 | Required                                                                                                                                                                                             | Description                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                            | [operations.ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormRequest](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form-request.md)   | :heavy_check_mark:                                                                                                                                                                                   | The request object to use for the request.                                                                                                                                                           |
| `security`                                                                                                                                                                                           | [operations.ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormSecurity](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form-security.md) | :heavy_check_mark:                                                                                                                                                                                   | The security requirements to use for the request.                                                                                                                                                    |
| `options`                                                                                                                                                                                            | RequestOptions                                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                   | Used to set various options for making HTTP requests.                                                                                                                                                |
| `options.fetchOptions`                                                                                                                                                                               | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                   | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                       |
| `options.retries`                                                                                                                                                                                    | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                   | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                     |

### Response

**Promise\<[operations.ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormResponse](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm

Use this Web API to load the Hosted Payment Page of a Payment Gateway service in a front-end system (mobile apps, landing pages) to capture a payment method’s details. The Web API will also result in adding the payment method for the contact as well, so after this call no further actions are needed for storing the payment method’s information in CRM.COM.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.HostedPagesSelfServiceResource_generateAddPaymentMethodForm" method="get" path="/self-service/v2/hosted_pages/payment_methods" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.hostedPages.comCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    currencyCode: "EUR",
    integrationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { hostedPagesComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm } from "crm/funcs/hosted-pages-com-crm-hosted-pages-self-service-resource-generate-add-payment-method-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await hostedPagesComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    currencyCode: "EUR",
    integrationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("hostedPagesComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                              | Type                                                                                                                                                                                                   | Required                                                                                                                                                                                               | Description                                                                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                                              | [operations.ComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodFormRequest](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-add-payment-method-form-request.md)   | :heavy_check_mark:                                                                                                                                                                                     | The request object to use for the request.                                                                                                                                                             |
| `security`                                                                                                                                                                                             | [operations.ComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodFormSecurity](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-add-payment-method-form-security.md) | :heavy_check_mark:                                                                                                                                                                                     | The security requirements to use for the request.                                                                                                                                                      |
| `options`                                                                                                                                                                                              | RequestOptions                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                     | Used to set various options for making HTTP requests.                                                                                                                                                  |
| `options.fetchOptions`                                                                                                                                                                                 | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                                | :heavy_minus_sign:                                                                                                                                                                                     | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.                         |
| `options.retries`                                                                                                                                                                                      | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                     | Enables retrying HTTP requests under certain failure conditions.                                                                                                                                       |

### Response

**Promise\<[operations.ComCrmHostedPagesSelfServiceResourceGenerateAddPaymentMethodFormResponse](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-add-payment-method-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmHostedPagesSelfServiceResourceGeneratePaymentForm

Web API used when consumers want to perform a payment using a card on file. It's vital to study the Payment Gateway's required contact information. Make sure that this required information is already specified for contacts that use this form to make payments/top-ups since this Web API does not forward/includes such info in the request!

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.HostedPagesSelfServiceResource_generatePaymentForm" method="get" path="/self-service/v2/hosted_pages/payments" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.hostedPages.comCrmHostedPagesSelfServiceResourceGeneratePaymentForm({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    amount: 23.4,
    currencyCode: "EUR",
    estimationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    integrationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    paymentMethodId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    type: "PAYMENT",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePaymentForm } from "crm/funcs/hosted-pages-com-crm-hosted-pages-self-service-resource-generate-payment-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePaymentForm(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    amount: 23.4,
    currencyCode: "EUR",
    estimationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    integrationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    paymentMethodId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
    type: "PAYMENT",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePaymentForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                          | Type                                                                                                                                                                               | Required                                                                                                                                                                           | Description                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                          | [operations.ComCrmHostedPagesSelfServiceResourceGeneratePaymentFormRequest](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payment-form-request.md)   | :heavy_check_mark:                                                                                                                                                                 | The request object to use for the request.                                                                                                                                         |
| `security`                                                                                                                                                                         | [operations.ComCrmHostedPagesSelfServiceResourceGeneratePaymentFormSecurity](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payment-form-security.md) | :heavy_check_mark:                                                                                                                                                                 | The security requirements to use for the request.                                                                                                                                  |
| `options`                                                                                                                                                                          | RequestOptions                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                 | Used to set various options for making HTTP requests.                                                                                                                              |
| `options.fetchOptions`                                                                                                                                                             | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                            | :heavy_minus_sign:                                                                                                                                                                 | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.     |
| `options.retries`                                                                                                                                                                  | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                 | Enables retrying HTTP requests under certain failure conditions.                                                                                                                   |

### Response

**Promise\<[operations.ComCrmHostedPagesSelfServiceResourceGeneratePaymentFormResponse](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payment-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmHostedPagesSelfServiceResourceGeneratePayoutForm

Web API used when consumers want to perform a payout. It's vital to study the Payment Gateway's required contact information. Make sure that this required information is already specified for contacts that use this form to make payouts since this Web API does not forward/includes such info in the request!

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.HostedPagesSelfServiceResource_generatePayoutForm" method="get" path="/self-service/v2/hosted_pages/payouts" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.hostedPages.comCrmHostedPagesSelfServiceResourceGeneratePayoutForm({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    amount: 23.4,
    currencyCode: "EUR",
    fullName: "John Doe",
    integrationId: "302fb9b0-d57c-4a07-ae0b-b7cbec934775",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePayoutForm } from "crm/funcs/hosted-pages-com-crm-hosted-pages-self-service-resource-generate-payout-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePayoutForm(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    amount: 23.4,
    currencyCode: "EUR",
    fullName: "John Doe",
    integrationId: "302fb9b0-d57c-4a07-ae0b-b7cbec934775",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("hostedPagesComCrmHostedPagesSelfServiceResourceGeneratePayoutForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                        | Type                                                                                                                                                                             | Required                                                                                                                                                                         | Description                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                        | [operations.ComCrmHostedPagesSelfServiceResourceGeneratePayoutFormRequest](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payout-form-request.md)   | :heavy_check_mark:                                                                                                                                                               | The request object to use for the request.                                                                                                                                       |
| `security`                                                                                                                                                                       | [operations.ComCrmHostedPagesSelfServiceResourceGeneratePayoutFormSecurity](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payout-form-security.md) | :heavy_check_mark:                                                                                                                                                               | The security requirements to use for the request.                                                                                                                                |
| `options`                                                                                                                                                                        | RequestOptions                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                               | Used to set various options for making HTTP requests.                                                                                                                            |
| `options.fetchOptions`                                                                                                                                                           | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                          | :heavy_minus_sign:                                                                                                                                                               | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.   |
| `options.retries`                                                                                                                                                                | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                               | Enables retrying HTTP requests under certain failure conditions.                                                                                                                 |

### Response

**Promise\<[operations.ComCrmHostedPagesSelfServiceResourceGeneratePayoutFormResponse](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-payout-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |