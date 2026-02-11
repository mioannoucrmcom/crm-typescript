# ~~PaymentForms~~

> [!WARNING]
> This SDK is **DEPRECATED**

## Overview

Payment Forms

### Available Operations

* [~~comCrmPaymentFormSelfServiceResourceGenerateAddCardForm~~](#comcrmpaymentformselfserviceresourcegenerateaddcardform) - Add Card :warning: **Deprecated**
* [~~comCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm~~](#comcrmpaymentformselfserviceresourcegeneratepasspaymentform) - Get Gift Pass Payment Form :warning: **Deprecated**
* [~~comCrmPaymentFormSelfServiceResourceGeneratePaymentForm~~](#comcrmpaymentformselfserviceresourcegeneratepaymentform) - Payment Form :warning: **Deprecated**

## ~~comCrmPaymentFormSelfServiceResourceGenerateAddCardForm~~

Web API used when consumers add a Card from a Landing page. The Web API forwards information of the card, along with the buyer details. In addition, the Web API integrates with the Payment Gateway service and request to load their payment form for an easy payment processing. To avoid any issues, it's vital to check the Payment Gateway service's mandatory information requirements, such as the buyer's email, phone, and address information, before triggering the Web API. 

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PaymentFormSelfServiceResource_generateAddCardForm" method="get" path="/self-service/v2/payment_forms/card" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.paymentForms.comCrmPaymentFormSelfServiceResourceGenerateAddCardForm({
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
import { paymentFormsComCrmPaymentFormSelfServiceResourceGenerateAddCardForm } from "crm/funcs/payment-forms-com-crm-payment-form-self-service-resource-generate-add-card-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await paymentFormsComCrmPaymentFormSelfServiceResourceGenerateAddCardForm(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    currencyCode: "EUR",
    integrationId: "2301a540-8f81-e4d2-7418-dfa714ac53ee",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("paymentFormsComCrmPaymentFormSelfServiceResourceGenerateAddCardForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                           | Type                                                                                                                                                                                | Required                                                                                                                                                                            | Description                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                           | [operations.ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormRequest](../../models/operations/com-crm-payment-form-self-service-resource-generate-add-card-form-request.md)   | :heavy_check_mark:                                                                                                                                                                  | The request object to use for the request.                                                                                                                                          |
| `security`                                                                                                                                                                          | [operations.ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormSecurity](../../models/operations/com-crm-payment-form-self-service-resource-generate-add-card-form-security.md) | :heavy_check_mark:                                                                                                                                                                  | The security requirements to use for the request.                                                                                                                                   |
| `options`                                                                                                                                                                           | RequestOptions                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                  | Used to set various options for making HTTP requests.                                                                                                                               |
| `options.fetchOptions`                                                                                                                                                              | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                             | :heavy_minus_sign:                                                                                                                                                                  | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.      |
| `options.retries`                                                                                                                                                                   | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                  | Enables retrying HTTP requests under certain failure conditions.                                                                                                                    |

### Response

**Promise\<[operations.ComCrmPaymentFormSelfServiceResourceGenerateAddCardFormResponse](../../models/operations/com-crm-payment-form-self-service-resource-generate-add-card-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## ~~comCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm~~

Web API used when consumers purchase Gift Passes from a Landing page. The Web API forwards information of the purchased pass, along with the buyer and receiver's details. In addition, the Web aPI integrates with the Payment Gateway service and request to load their payment form for an easy payment processing. To avoid any issues, it's vital to check the Payment Gateway service's mandatory information requirements, such as the buyer's email, phone, and address information, before triggering the Web API. 

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PaymentFormSelfServiceResource_generatePassPaymentForm" method="post" path="/self-service/v2/payment_forms/pass" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.paymentForms.comCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm({
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
import { paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm } from "crm/funcs/payment-forms-com-crm-payment-form-self-service-resource-generate-pass-payment-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm(crm, {
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
    console.log("paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePassPaymentForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                                   | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                                   | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormRequest](../../models/operations/com-crm-payment-form-self-service-resource-generate-pass-payment-form-request.md)   | :heavy_check_mark:                                                                                                                                                                          | The request object to use for the request.                                                                                                                                                  |
| `security`                                                                                                                                                                                  | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormSecurity](../../models/operations/com-crm-payment-form-self-service-resource-generate-pass-payment-form-security.md) | :heavy_check_mark:                                                                                                                                                                          | The security requirements to use for the request.                                                                                                                                           |
| `options`                                                                                                                                                                                   | RequestOptions                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                          | Used to set various options for making HTTP requests.                                                                                                                                       |
| `options.fetchOptions`                                                                                                                                                                      | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                                     | :heavy_minus_sign:                                                                                                                                                                          | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.              |
| `options.retries`                                                                                                                                                                           | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                          | Enables retrying HTTP requests under certain failure conditions.                                                                                                                            |

### Response

**Promise\<[operations.ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormResponse](../../models/operations/com-crm-payment-form-self-service-resource-generate-pass-payment-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## ~~comCrmPaymentFormSelfServiceResourceGeneratePaymentForm~~

Web API used when consumers want to perform a payment using a card on file. It's vital to study the Payment Gateway's required contact information. Make sure that this required information is already specified for contacts that use this form to make payments/top-ups since this Web API does not forward/includes such info in the request!

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PaymentFormSelfServiceResource_generatePaymentForm" method="get" path="/self-service/v2/payment_forms/payment" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.paymentForms.comCrmPaymentFormSelfServiceResourceGeneratePaymentForm({
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
import { paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePaymentForm } from "crm/funcs/payment-forms-com-crm-payment-form-self-service-resource-generate-payment-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePaymentForm(crm, {
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
    console.log("paymentFormsComCrmPaymentFormSelfServiceResourceGeneratePaymentForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                          | Type                                                                                                                                                                               | Required                                                                                                                                                                           | Description                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                          | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormRequest](../../models/operations/com-crm-payment-form-self-service-resource-generate-payment-form-request.md)   | :heavy_check_mark:                                                                                                                                                                 | The request object to use for the request.                                                                                                                                         |
| `security`                                                                                                                                                                         | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormSecurity](../../models/operations/com-crm-payment-form-self-service-resource-generate-payment-form-security.md) | :heavy_check_mark:                                                                                                                                                                 | The security requirements to use for the request.                                                                                                                                  |
| `options`                                                                                                                                                                          | RequestOptions                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                 | Used to set various options for making HTTP requests.                                                                                                                              |
| `options.fetchOptions`                                                                                                                                                             | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                            | :heavy_minus_sign:                                                                                                                                                                 | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.     |
| `options.retries`                                                                                                                                                                  | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                 | Enables retrying HTTP requests under certain failure conditions.                                                                                                                   |

### Response

**Promise\<[operations.ComCrmPaymentFormSelfServiceResourceGeneratePaymentFormResponse](../../models/operations/com-crm-payment-form-self-service-resource-generate-payment-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |