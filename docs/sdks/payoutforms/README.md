# ~~PayoutForms~~

> [!WARNING]
> This SDK is **DEPRECATED**

## Overview

Payout Forms

### Available Operations

* [~~comCrmPayoutFormSelfServiceResourceGeneratePayoutForm~~](#comcrmpayoutformselfserviceresourcegeneratepayoutform) - Payout Form :warning: **Deprecated**

## ~~comCrmPayoutFormSelfServiceResourceGeneratePayoutForm~~

Web API used when consumers want to perform a payout. It's vital to study the Payment Gateway's required contact information. Make sure that this required information is already specified for contacts that use this form to make payouts since this Web API does not forward/includes such info in the request!

> :warning: **DEPRECATED**: This will be removed in a future release, please migrate away from it as soon as possible.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PayoutFormSelfServiceResource_generatePayoutForm" method="get" path="/self-service/v2/payout_forms/payout" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.payoutForms.comCrmPayoutFormSelfServiceResourceGeneratePayoutForm({
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
import { payoutFormsComCrmPayoutFormSelfServiceResourceGeneratePayoutForm } from "crm/funcs/payout-forms-com-crm-payout-form-self-service-resource-generate-payout-form.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await payoutFormsComCrmPayoutFormSelfServiceResourceGeneratePayoutForm(crm, {
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
    console.log("payoutFormsComCrmPayoutFormSelfServiceResourceGeneratePayoutForm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPayoutFormSelfServiceResourceGeneratePayoutFormRequest](../../models/operations/com-crm-payout-form-self-service-resource-generate-payout-form-request.md)   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmPayoutFormSelfServiceResourceGeneratePayoutFormSecurity](../../models/operations/com-crm-payout-form-self-service-resource-generate-payout-form-security.md) | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPayoutFormSelfServiceResourceGeneratePayoutFormResponse](../../models/operations/com-crm-payout-form-self-service-resource-generate-payout-form-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |