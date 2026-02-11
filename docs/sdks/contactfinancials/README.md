# ContactFinancials

## Overview

Contact Financials APIs

### Available Operations

* [comCrmContactSelfServiceResourceGetClientToken](#comcrmcontactselfserviceresourcegetclienttoken) - Get a Contact Client Token
* [comCrmPaymentIntentSelfServiceResourceSetUpIntents](#comcrmpaymentintentselfserviceresourcesetupintents) - Create Intent
* [comCrmPaymentSelfServiceResourceCreate](#comcrmpaymentselfserviceresourcecreate) - Create Payment
* [comCrmPayoutSelfServiceResourceCreate](#comcrmpayoutselfserviceresourcecreate) - Create Payout
* [comCrmSettlementTransactionSelfServiceResourceList](#comcrmsettlementtransactionselfserviceresourcelist) - Get Settlement Transactions
* [comCrmSettlementTransactionSelfServiceResourceGetMetrics](#comcrmsettlementtransactionselfserviceresourcegetmetrics) - Get Settlement Transactions Metrics
* [comCrmTopUpSelfServiceResourceCreate](#comcrmtopupselfserviceresourcecreate) - Create Top-up
* [comCrmTransferSelfServiceResourceCreate](#comcrmtransferselfserviceresourcecreate) - Transfer Money
* [comCrmTransferSelfServiceResourceCreateTransferBulk](#comcrmtransferselfserviceresourcecreatetransferbulk) - Transfer Money in Bulk

## comCrmContactSelfServiceResourceGetClientToken

Get a Contact Client Token

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getClientToken" method="get" path="/self-service/v2/contacts/{id}/client_token" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.contactFinancials.comCrmContactSelfServiceResourceGetClientToken({
    id: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmContactSelfServiceResourceGetClientToken } from "crmcom/funcs/contact-financials-com-crm-contact-self-service-resource-get-client-token.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmContactSelfServiceResourceGetClientToken(crmcom, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactFinancialsComCrmContactSelfServiceResourceGetClientToken failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetClientTokenRequest](../../models/operations/com-crm-contact-self-service-resource-get-client-token-request.md)                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPaymentIntentSelfServiceResourceSetUpIntents

Set up a new payment intent for a specific contact. A Payment intent represents the contact's intention to make a payment using one of the registered online payment methods. The response varies depending on the Payment Gateway service that processes the intent.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PaymentIntentSelfServiceResource_setUpIntents" method="post" path="/self-service/v2/contacts/{id}/intents" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmPaymentIntentSelfServiceResourceSetUpIntents({
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      integrationId: "2BD9C84FA60F9FE407140E20F707726A",
      paymentMethodId: "3BD9C84FA60F9FE407140E20F707726A",
      capture: "ON_HOLD",
      amount: 9.99,
      currencyCode: "EUR",
      statementInfo: "Payment for Order O125435 - Date 01.01.2010",
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
import { contactFinancialsComCrmPaymentIntentSelfServiceResourceSetUpIntents } from "crmcom/funcs/contact-financials-com-crm-payment-intent-self-service-resource-set-up-intents.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmPaymentIntentSelfServiceResourceSetUpIntents(crmcom, {
    id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    body: {
      integrationId: "2BD9C84FA60F9FE407140E20F707726A",
      paymentMethodId: "3BD9C84FA60F9FE407140E20F707726A",
      capture: "ON_HOLD",
      amount: 9.99,
      currencyCode: "EUR",
      statementInfo: "Payment for Order O125435 - Date 01.01.2010",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmPaymentIntentSelfServiceResourceSetUpIntents failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPaymentIntentSelfServiceResourceSetUpIntentsRequest](../../models/operations/com-crm-payment-intent-self-service-resource-set-up-intents-request.md)         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPaymentIntentSelfServiceResourceSetUpIntentsResponse](../../models/operations/com-crm-payment-intent-self-service-resource-set-up-intents-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPaymentSelfServiceResourceCreate

Create a new Payment transaction for a Contact. The Payment will be issued as Posted.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PaymentSelfServiceResource_create" method="post" path="/self-service/v2/payments" example="Create Payment" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contactFinancials.comCrmPaymentSelfServiceResourceCreate({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    accountId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    code: "1234567891234567",
    clientSecret: "",
    amount: 1,
    currencyCode: "EUR",
    contactId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    paymentMethod: {
      id: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      type: "CARD",
    },
    invoicesPaid: [
      {
        id: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
    ],
    externalPayable: [
      {
        reference: "INV00001011",
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
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmPaymentSelfServiceResourceCreate } from "crmcom/funcs/contact-financials-com-crm-payment-self-service-resource-create.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactFinancialsComCrmPaymentSelfServiceResourceCreate(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    accountId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
    code: "1234567891234567",
    clientSecret: "",
    amount: 1,
    currencyCode: "EUR",
    contactId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    paymentMethod: {
      id: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      type: "CARD",
    },
    invoicesPaid: [
      {
        id: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
    ],
    externalPayable: [
      {
        reference: "INV00001011",
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
    console.log("contactFinancialsComCrmPaymentSelfServiceResourceCreate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPaymentSelfServiceResourceCreateRequest](../../models/operations/com-crm-payment-self-service-resource-create-request.md)                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmPaymentSelfServiceResourceCreateSecurity](../../models/operations/com-crm-payment-self-service-resource-create-security.md)                                  | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPaymentSelfServiceResourceCreateResponse](../../models/operations/com-crm-payment-self-service-resource-create-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmPayoutSelfServiceResourceCreate

Create a new payout financial transaction against a wallet

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.PayoutSelfServiceResource_create" method="post" path="/self-service/v2/payouts" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contactFinancials.comCrmPayoutSelfServiceResourceCreate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    walletId: "55063493-910c-5366-216f-31065832bdb5",
    amount: 200,
    paymentMethod: {
      id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      type: "CARD",
    },
    notes: "Payout due to wrong payment amount",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmPayoutSelfServiceResourceCreate } from "crmcom/funcs/contact-financials-com-crm-payout-self-service-resource-create.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactFinancialsComCrmPayoutSelfServiceResourceCreate(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    walletId: "55063493-910c-5366-216f-31065832bdb5",
    amount: 200,
    paymentMethod: {
      id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      type: "CARD",
    },
    notes: "Payout due to wrong payment amount",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmPayoutSelfServiceResourceCreate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmPayoutSelfServiceResourceCreateRequest](../../models/operations/com-crm-payout-self-service-resource-create-request.md)                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmPayoutSelfServiceResourceCreateSecurity](../../models/operations/com-crm-payout-self-service-resource-create-security.md)                                    | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmPayoutSelfServiceResourceCreateResponse](../../models/operations/com-crm-payout-self-service-resource-create-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSettlementTransactionSelfServiceResourceList

Retrieve the settlement transactions related to B2B Settlement

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SettlementTransactionSelfServiceResource_list" method="get" path="/self-service/v2/settlement_transactions" example="CREATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmSettlementTransactionSelfServiceResourceList({
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
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
import { contactFinancialsComCrmSettlementTransactionSelfServiceResourceList } from "crmcom/funcs/contact-financials-com-crm-settlement-transaction-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmSettlementTransactionSelfServiceResourceList(crmcom, {
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmSettlementTransactionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.SettlementTransactionSelfServiceResource_list" method="get" path="/self-service/v2/settlement_transactions" example="NAME" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmSettlementTransactionSelfServiceResourceList({
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
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
import { contactFinancialsComCrmSettlementTransactionSelfServiceResourceList } from "crmcom/funcs/contact-financials-com-crm-settlement-transaction-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmSettlementTransactionSelfServiceResourceList(crmcom, {
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmSettlementTransactionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SettlementTransactionSelfServiceResource_list" method="get" path="/self-service/v2/settlement_transactions" example="SCHEDULED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmSettlementTransactionSelfServiceResourceList({
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
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
import { contactFinancialsComCrmSettlementTransactionSelfServiceResourceList } from "crmcom/funcs/contact-financials-com-crm-settlement-transaction-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmSettlementTransactionSelfServiceResourceList(crmcom, {
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmSettlementTransactionSelfServiceResourceList failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.SettlementTransactionSelfServiceResource_list" method="get" path="/self-service/v2/settlement_transactions" example="UPDATED_DATE" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmSettlementTransactionSelfServiceResourceList({
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
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
import { contactFinancialsComCrmSettlementTransactionSelfServiceResourceList } from "crmcom/funcs/contact-financials-com-crm-settlement-transaction-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmSettlementTransactionSelfServiceResourceList(crmcom, {
    accountJournalEntryId: "4c156688-4d53-d0e4-e483-1809cacaaaca",
    accountingType: "CREDIT",
    currencyCode: "EUR",
    settlementType: "AWARD",
    state: "POSTED",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmSettlementTransactionSelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmSettlementTransactionSelfServiceResourceListRequest](../../models/operations/com-crm-settlement-transaction-self-service-resource-list-request.md)           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmSettlementTransactionSelfServiceResourceListResponse](../../models/operations/com-crm-settlement-transaction-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmSettlementTransactionSelfServiceResourceGetMetrics

Retrieve some metrics related to the settlement transactions

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.SettlementTransactionSelfServiceResource_getMetrics" method="get" path="/self-service/v2/settlement_transactions/metrics" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactFinancials.comCrmSettlementTransactionSelfServiceResourceGetMetrics();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmSettlementTransactionSelfServiceResourceGetMetrics } from "crmcom/funcs/contact-financials-com-crm-settlement-transaction-self-service-resource-get-metrics.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactFinancialsComCrmSettlementTransactionSelfServiceResourceGetMetrics(crmcom);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmSettlementTransactionSelfServiceResourceGetMetrics failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                         | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                         | [operations.ComCrmSettlementTransactionSelfServiceResourceGetMetricsRequest](../../models/operations/com-crm-settlement-transaction-self-service-resource-get-metrics-request.md) | :heavy_check_mark:                                                                                                                                                                | The request object to use for the request.                                                                                                                                        |
| `options`                                                                                                                                                                         | RequestOptions                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                | Used to set various options for making HTTP requests.                                                                                                                             |
| `options.fetchOptions`                                                                                                                                                            | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                           | :heavy_minus_sign:                                                                                                                                                                | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.    |
| `options.retries`                                                                                                                                                                 | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                | Enables retrying HTTP requests under certain failure conditions.                                                                                                                  |

### Response

**Promise\<[operations.ComCrmSettlementTransactionSelfServiceResourceGetMetricsResponse](../../models/operations/com-crm-settlement-transaction-self-service-resource-get-metrics-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmTopUpSelfServiceResourceCreate

Create a new Topup for a Wallet

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.TopUpSelfServiceResource_create" method="post" path="/self-service/v2/topups" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contactFinancials.comCrmTopUpSelfServiceResourceCreate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    topupDate: 14423423,
    amount: 1,
    code: "1234567891234567",
    paymentMethod: {
      id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      type: "CARD",
    },
    clientSecret: "",
    commercePoolId: "",
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
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmTopUpSelfServiceResourceCreate } from "crmcom/funcs/contact-financials-com-crm-top-up-self-service-resource-create.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactFinancialsComCrmTopUpSelfServiceResourceCreate(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    topupDate: 14423423,
    amount: 1,
    code: "1234567891234567",
    paymentMethod: {
      id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      type: "CARD",
    },
    clientSecret: "",
    commercePoolId: "",
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
    console.log("contactFinancialsComCrmTopUpSelfServiceResourceCreate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmTopUpSelfServiceResourceCreateRequest](../../models/operations/com-crm-top-up-self-service-resource-create-request.md)                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmTopUpSelfServiceResourceCreateSecurity](../../models/operations/com-crm-top-up-self-service-resource-create-security.md)                                     | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmTopUpSelfServiceResourceCreateResponse](../../models/operations/com-crm-top-up-self-service-resource-create-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmTransferSelfServiceResourceCreate

Transfers an amount of money from one account or wallet to another account or wallet. A single transfer can be created per Web API call. An amount of money can be transferred to another account/wallet of the same contact who owns the origin account/wallet or transferred to another contact's account/wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.TransferSelfServiceResource_create" method="post" path="/self-service/v2/transfers" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.contactFinancials.comCrmTransferSelfServiceResourceCreate({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    origin: {
      accountId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      walletId: "A65ACCE45B2E68DFDCAD1E31269B76D7",
    },
    destination: {
      accountId: "CE45B2E68DFDCAD1E31269B76D7A65AC",
      walletId: "B76D7A65ACCCAD1E31269E45B2E68DFD",
    },
    transferDate: 1620999582,
    amount: 9.99,
    code: "1234567891234567",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmTransferSelfServiceResourceCreate } from "crmcom/funcs/contact-financials-com-crm-transfer-self-service-resource-create.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactFinancialsComCrmTransferSelfServiceResourceCreate(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    origin: {
      accountId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
      walletId: "A65ACCE45B2E68DFDCAD1E31269B76D7",
    },
    destination: {
      accountId: "CE45B2E68DFDCAD1E31269B76D7A65AC",
      walletId: "B76D7A65ACCCAD1E31269E45B2E68DFD",
    },
    transferDate: 1620999582,
    amount: 9.99,
    code: "1234567891234567",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactFinancialsComCrmTransferSelfServiceResourceCreate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmTransferSelfServiceResourceCreateRequest](../../models/operations/com-crm-transfer-self-service-resource-create-request.md)                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmTransferSelfServiceResourceCreateSecurity](../../models/operations/com-crm-transfer-self-service-resource-create-security.md)                                | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmTransferSelfServiceResourceCreateResponse](../../models/operations/com-crm-transfer-self-service-resource-create-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmTransferSelfServiceResourceCreateTransferBulk

Transfers an amount of money from one account or wallet to another account or wallet in bulk. A single transaction will be created for each transfer request. An amount of money can be transferred to another account/wallet of the same contact who owns the origin account/wallet or transferred to another contact's account/wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.TransferSelfServiceResource_createTransferBulk" method="post" path="/self-service/v2/transfers/bulk" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  await crmcom.contactFinancials.comCrmTransferSelfServiceResourceCreateTransferBulk({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, [
    {
      origin: {
        accountId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
        walletId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
      destination: {
        accountId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
        walletId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
      transferDate: 1620999582,
      amount: 9.99,
      code: "1234567891234567",
      commercePoolId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    },
  ]);


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactFinancialsComCrmTransferSelfServiceResourceCreateTransferBulk } from "crmcom/funcs/contact-financials-com-crm-transfer-self-service-resource-create-transfer-bulk.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await contactFinancialsComCrmTransferSelfServiceResourceCreateTransferBulk(crmcom, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, [
    {
      origin: {
        accountId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
        walletId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
      destination: {
        accountId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
        walletId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
      },
      transferDate: 1620999582,
      amount: 9.99,
      code: "1234567891234567",
      commercePoolId: "ab5f8b2e-092f-4848-8f46-31df1c014060",
    },
  ]);
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactFinancialsComCrmTransferSelfServiceResourceCreateTransferBulk failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.RequestBody[]](../../models/.md)                                                                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmTransferSelfServiceResourceCreateTransferBulkSecurity](../../models/operations/com-crm-transfer-self-service-resource-create-transfer-bulk-security.md)      | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |