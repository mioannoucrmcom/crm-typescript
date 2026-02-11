# ContactWallet

## Overview

Contact Wallet

### Available Operations

* [comCrmContactSelfServiceResourceSetUpWallet](#comcrmcontactselfserviceresourcesetupwallet) - Create Wallet
* [comCrmWalletSelfServiceResourceRequestOTP](#comcrmwalletselfserviceresourcerequestotp) - Request Wallet One Time Password
* [comCrmWalletSelfServiceResourceVerifyWalletExists](#comcrmwalletselfserviceresourceverifywalletexists) - Verify Wallet identity Existence
* [comCrmWalletSelfServiceResourceGetSingle](#comcrmwalletselfserviceresourcegetsingle) - Get Wallet
* [comCrmWalletSelfServiceResourceUpdate](#comcrmwalletselfserviceresourceupdate) - Update Wallet
* [comCrmWalletSelfServiceResourceGetWalletCode](#comcrmwalletselfserviceresourcegetwalletcode) - Get Wallet Code
* [comCrmWalletSelfServiceResourceGetBalances](#comcrmwalletselfserviceresourcegetbalances) - List Wallet Commerce Balances
* [comCrmWalletSelfServiceResourceListWalletJournals](#comcrmwalletselfserviceresourcelistwalletjournals) - List Wallet Journals
* [comCrmWalletSelfServiceResourceGetWalletLimits](#comcrmwalletselfserviceresourcegetwalletlimits) - Get Wallet Limits
* [comCrmWalletSelfServiceResourceUpdateLimits](#comcrmwalletselfserviceresourceupdatelimits) - Update Wallet Limits
* [comCrmWalletSelfServiceResourceGetWalletSummarisedTotals](#comcrmwalletselfserviceresourcegetwalletsummarisedtotals) - List Wallet Summarised Totals
* [comCrmWalletSelfServiceResourceGetWalletTopUpSettings](#comcrmwalletselfserviceresourcegetwallettopupsettings) - Get Wallet Top-up Settings
* [comCrmWalletSelfServiceResourceGetTransactions](#comcrmwalletselfserviceresourcegettransactions) - List Wallet (Journal) Transactions

## comCrmContactSelfServiceResourceSetUpWallet

Set ups the Wallet for the contact by either creating a new one or linking the wallet to the contact.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_setUpWallet" method="post" path="/self-service/v2/contacts/{id}/wallets" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactWallet.comCrmContactSelfServiceResourceSetUpWallet({
    id: "<id>",
    body: {
      otp: "146123",
      code: "5444406970005411",
      identity: {
        type: "PHONE",
        value: "some_email@email.com",
      },
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmContactSelfServiceResourceSetUpWallet } from "crm/funcs/contact-wallet-com-crm-contact-self-service-resource-set-up-wallet.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmContactSelfServiceResourceSetUpWallet(crm, {
    id: "<id>",
    body: {
      otp: "146123",
      code: "5444406970005411",
      identity: {
        type: "PHONE",
        value: "some_email@email.com",
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactWalletComCrmContactSelfServiceResourceSetUpWallet failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceSetUpWalletRequest](../../models/operations/com-crm-contact-self-service-resource-set-up-wallet-request.md)                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceRequestOTP

Request Wallet One Time Password

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_requestOTP" method="post" path="/self-service/v2/wallets/otp" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactWallet.comCrmWalletSelfServiceResourceRequestOTP({
    identity: {
      type: "PHONE",
      value: "some_email@email.com",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceRequestOTP } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-request-otp.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceRequestOTP(crm, {
    identity: {
      type: "PHONE",
      value: "some_email@email.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceRequestOTP failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceRequestOTPRequest](../../models/operations/com-crm-wallet-self-service-resource-request-otp-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceVerifyWalletExists

Verify the existence of a wallet using either their email or phone as wallet identity. The result is a boolean value.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_verifyWalletExists" method="get" path="/self-service/v2/wallets/wallet_exists" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceVerifyWalletExists({
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "EMAIL",
    value: "99123456",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceVerifyWalletExists } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-verify-wallet-exists.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceVerifyWalletExists(crm, {
    publicAPIKey: process.env["CRM_PUBLIC_API_KEY"] ?? "",
  }, {
    type: "EMAIL",
    value: "99123456",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceVerifyWalletExists failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceVerifyWalletExistsRequest](../../models/operations/com-crm-wallet-self-service-resource-verify-wallet-exists-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmWalletSelfServiceResourceVerifyWalletExistsSecurity](../../models/operations/com-crm-wallet-self-service-resource-verify-wallet-exists-security.md)          | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceVerifyWalletExistsResponse](../../models/operations/com-crm-wallet-self-service-resource-verify-wallet-exists-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetSingle

Retrieves detailed information of a single Wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getSingle" method="get" path="/self-service/v2/wallets/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetSingle({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetSingle } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-single.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetSingle(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetSingle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetSingleRequest](../../models/operations/com-crm-wallet-self-service-resource-get-single-request.md)                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmWalletSelfServiceResourceGetSingleSecurity](../../models/operations/com-crm-wallet-self-service-resource-get-single-security.md)                             | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetSingleResponse](../../models/operations/com-crm-wallet-self-service-resource-get-single-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceUpdate

Updates a single Wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_update" method="put" path="/self-service/v2/wallets/{id}" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceUpdate({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "3ac0809f-ed91-4b68-b912-5bd6064d901e",
    body: {
      autoTopup: {
        threshold: 0.01,
        amount: 10.5,
        paymentMethod: {
          id: "",
          type: "CARD",
        },
      },
      termedTopup: {
        amount: 10.5,
        frequency: "0 0 12 * * ?",
        paymentMethod: {
          type: "CARD",
        },
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
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceUpdate } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-update.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceUpdate(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "3ac0809f-ed91-4b68-b912-5bd6064d901e",
    body: {
      autoTopup: {
        threshold: 0.01,
        amount: 10.5,
        paymentMethod: {
          id: "",
          type: "CARD",
        },
      },
      termedTopup: {
        amount: 10.5,
        frequency: "0 0 12 * * ?",
        paymentMethod: {
          type: "CARD",
        },
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceUpdate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceUpdateRequest](../../models/operations/com-crm-wallet-self-service-resource-update-request.md)                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmWalletSelfServiceResourceUpdateSecurity](../../models/operations/com-crm-wallet-self-service-resource-update-security.md)                                    | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceUpdateResponse](../../models/operations/com-crm-wallet-self-service-resource-update-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetWalletCode

Depending on the business’s wallet settings, the API returns either a dynamically generated wallet code - which is regularly refreshed for security, or a static wallet code - which remains constant. The wallet code is used when a contact checks in or generates an OTP to spend wallet funds when purchasing via the Contact App.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getWalletCode" method="get" path="/self-service/v2/wallets/{id}/code" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetWalletCode({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetWalletCode } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-wallet-code.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetWalletCode(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetWalletCode failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetWalletCodeRequest](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-code-request.md)                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetWalletCodeResponse](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-code-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetBalances

Get the wallet’s balances split per commerce pool in descending order based on amount

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getBalances" method="get" path="/self-service/v2/wallets/{id}/commerce_balances" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetBalances({
    id: "acf8b8ac-a325-a644-c866-a6c9d62ff11b",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    isActive: true,
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetBalances } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-balances.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetBalances(crm, {
    id: "acf8b8ac-a325-a644-c866-a6c9d62ff11b",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    isActive: true,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetBalances failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetBalancesRequest](../../models/operations/com-crm-wallet-self-service-resource-get-balances-request.md)                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetBalancesResponse](../../models/operations/com-crm-wallet-self-service-resource-get-balances-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceListWalletJournals

Retrieve a list of wallet journals.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_listWalletJournals" method="get" path="/self-service/v2/wallets/{id}/journals" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceListWalletJournals({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceListWalletJournals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-list-wallet-journals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceListWalletJournals(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceListWalletJournals failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_listWalletJournals" method="get" path="/self-service/v2/wallets/{id}/journals" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceListWalletJournals({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceListWalletJournals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-list-wallet-journals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceListWalletJournals(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceListWalletJournals failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_listWalletJournals" method="get" path="/self-service/v2/wallets/{id}/journals" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceListWalletJournals({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceListWalletJournals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-list-wallet-journals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceListWalletJournals(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceListWalletJournals failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_listWalletJournals" method="get" path="/self-service/v2/wallets/{id}/journals" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceListWalletJournals({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceListWalletJournals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-list-wallet-journals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceListWalletJournals(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceListWalletJournals failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_listWalletJournals" method="get" path="/self-service/v2/wallets/{id}/journals" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceListWalletJournals({
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceListWalletJournals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-list-wallet-journals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceListWalletJournals(crm, {
    id: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    commercePoolId: "234fbc54-bc32-1990-ce59-76c45e6377a8",
    includeUnallocatedCredit: true,
    isCommerce: true,
    isOpen: true,
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    transactionType: "SETTLEMENT_PROCESS",
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceListWalletJournals failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceListWalletJournalsRequest](../../models/operations/com-crm-wallet-self-service-resource-list-wallet-journals-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceListWalletJournalsResponse](../../models/operations/com-crm-wallet-self-service-resource-list-wallet-journals-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetWalletLimits

Returns a list of wallet limit rules as these are specified by the contact. A limit rule determines conditions of how much wallet money can be spent for various transactions.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getWalletLimits" method="get" path="/self-service/v2/wallets/{id}/limits" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetWalletLimits({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetWalletLimits } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-wallet-limits.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetWalletLimits(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetWalletLimits failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetWalletLimitsRequest](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-limits-request.md)                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmWalletSelfServiceResourceGetWalletLimitsSecurity](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-limits-security.md)                | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetWalletLimitsResponse](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-limits-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceUpdateLimits

Update a wallets limits. Multiple rules can be updated, each one having a unique name. For each rule specify at least one limit setting to change i.e. minimum and maximum number of transactions with in a period and optionally which types of transactions.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_updateLimits" method="put" path="/self-service/v2/wallets/{id}/limits" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceUpdateLimits({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "3ac0809f-ed91-4b68-b912-5bd6064d901e",
    body: {
      limitRules: [
        {
          name: "Monthly topups",
          maximumNumber: 1,
          maximumAmount: 200,
          period: "DAILY",
          appliesFor: [
            "DEBIT",
          ],
          currencyCode: "BIF",
        },
      ],
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
import { contactWalletComCrmWalletSelfServiceResourceUpdateLimits } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-update-limits.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceUpdateLimits(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "3ac0809f-ed91-4b68-b912-5bd6064d901e",
    body: {
      limitRules: [
        {
          name: "Monthly topups",
          maximumNumber: 1,
          maximumAmount: 200,
          period: "DAILY",
          appliesFor: [
            "DEBIT",
          ],
          currencyCode: "BIF",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceUpdateLimits failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceUpdateLimitsRequest](../../models/operations/com-crm-wallet-self-service-resource-update-limits-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmWalletSelfServiceResourceUpdateLimitsSecurity](../../models/operations/com-crm-wallet-self-service-resource-update-limits-security.md)                       | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceUpdateLimitsResponse](../../models/operations/com-crm-wallet-self-service-resource-update-limits-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetWalletSummarisedTotals

Get the summarised totals for wallet transactions, grouped per transaction type and for a specific period of time. Only transactions conducted in the currency of the Business Pocket are taken into account. 
<br></br>
 Transactions are grouped as follows:
<br></br><table>
  <tr>
    <th>GROUP</th>
    <th>FINANCIAL TRANSACTION TYPE</th>
  </tr>
  <tr>
    <td>Top-ups</td>
    <td>PAYMENT, PASS_REDEMPTION, TOP_UP</td>
  </tr>
  <tr>
    <td>Spent</td>
    <td>B2B_SPEND, SPEND, USE_WALLET_FUNDS, WALLET_PAYMENT</td>
  </tr>
  <tr>
    <td>Sent</td>
    <td>TRANSFER, WALLET_SHARING</td>
  </tr>
  <tr>
    <td>Received</td>
    <td>TRANSFER, WALLET_SHARING</td>
  </tr>
  <tr>
    <td>Awarded</td>
    <td>AWARD, PURCHASE ACHIEVEMENT</td>
  </tr>
    <td>Redeemed</td>
    <td>REDEEM</td>
  </tr>
    <td>Donations</td>
    <td>DONATION</td>
  </tr>
    <td>Payouts</td>
    <td>PAYOUT</td>
  </tr>
</table>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getWalletSummarisedTotals" method="get" path="/self-service/v2/wallets/{id}/summarised_totals" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetWalletSummarisedTotals({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetWalletSummarisedTotals } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-wallet-summarised-totals.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetWalletSummarisedTotals(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetWalletSummarisedTotals failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                            | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                            | [operations.ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsRequest](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-summarised-totals-request.md)   | :heavy_check_mark:                                                                                                                                                                   | The request object to use for the request.                                                                                                                                           |
| `security`                                                                                                                                                                           | [operations.ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsSecurity](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-summarised-totals-security.md) | :heavy_check_mark:                                                                                                                                                                   | The security requirements to use for the request.                                                                                                                                    |
| `options`                                                                                                                                                                            | RequestOptions                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                   | Used to set various options for making HTTP requests.                                                                                                                                |
| `options.fetchOptions`                                                                                                                                                               | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                              | :heavy_minus_sign:                                                                                                                                                                   | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.       |
| `options.retries`                                                                                                                                                                    | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                   | Enables retrying HTTP requests under certain failure conditions.                                                                                                                     |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsResponse](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-summarised-totals-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetWalletTopUpSettings

Retrieves the wallet's Auto and Termed Top-up settings, as these are specified by the contact. If nothing is specified, then no automated or termed top-ups are performed since contacts must opt-in to such process by specifying this piece of information.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getWalletTopUpSettings" method="get" path="/self-service/v2/wallets/{id}/topup_settings" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm();

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetWalletTopUpSettings({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactWalletComCrmWalletSelfServiceResourceGetWalletTopUpSettings } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-wallet-top-up-settings.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore();

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetWalletTopUpSettings(crm, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetWalletTopUpSettings failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                       | Type                                                                                                                                                                            | Required                                                                                                                                                                        | Description                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                       | [operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsRequest](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-request.md)   | :heavy_check_mark:                                                                                                                                                              | The request object to use for the request.                                                                                                                                      |
| `security`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsSecurity](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-security.md) | :heavy_check_mark:                                                                                                                                                              | The security requirements to use for the request.                                                                                                                               |
| `options`                                                                                                                                                                       | RequestOptions                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                              | Used to set various options for making HTTP requests.                                                                                                                           |
| `options.fetchOptions`                                                                                                                                                          | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                         | :heavy_minus_sign:                                                                                                                                                              | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.  |
| `options.retries`                                                                                                                                                               | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                              | Enables retrying HTTP requests under certain failure conditions.                                                                                                                |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsResponse](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletSelfServiceResourceGetTransactions

Get all wallet journal transactions for a specific wallet with amount information as well as reasoning on how they were originated.

### Example Usage: CREATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getTransactions" method="get" path="/self-service/v2/wallets/{id}/transactions" example="CREATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetTransactions({
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceGetTransactions } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-transactions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetTransactions(crm, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetTransactions failed:", res.error);
  }
}

run();
```
### Example Usage: Example 1

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getTransactions" method="get" path="/self-service/v2/wallets/{id}/transactions" example="Example 1" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetTransactions({
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceGetTransactions } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-transactions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetTransactions(crm, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
    includeTotal: true,
    size: 100,
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetTransactions failed:", res.error);
  }
}

run();
```
### Example Usage: NAME

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getTransactions" method="get" path="/self-service/v2/wallets/{id}/transactions" example="NAME" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetTransactions({
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceGetTransactions } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-transactions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetTransactions(crm, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "NAME",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetTransactions failed:", res.error);
  }
}

run();
```
### Example Usage: SCHEDULED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getTransactions" method="get" path="/self-service/v2/wallets/{id}/transactions" example="SCHEDULED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetTransactions({
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceGetTransactions } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-transactions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetTransactions(crm, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "SCHEDULED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetTransactions failed:", res.error);
  }
}

run();
```
### Example Usage: UPDATED_DATE

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletSelfServiceResource_getTransactions" method="get" path="/self-service/v2/wallets/{id}/transactions" example="UPDATED_DATE" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactWallet.comCrmWalletSelfServiceResourceGetTransactions({
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
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
import { contactWalletComCrmWalletSelfServiceResourceGetTransactions } from "crm/funcs/contact-wallet-com-crm-wallet-self-service-resource-get-transactions.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactWalletComCrmWalletSelfServiceResourceGetTransactions(crm, {
    id: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    communityMemberId: "f76f96fc-22da-4f68-44d2-b9aeffa65d0f",
    isWalletFee: true,
    postedOnGt: 1618395497,
    postedOnGte: 1618395497,
    postedOnLt: 1618395497,
    postedOnLte: 1618395497,
    type: "CREDIT",
    includeTotal: true,
    size: 100,
    sort: "UPDATED_DATE",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactWalletComCrmWalletSelfServiceResourceGetTransactions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetTransactionsRequest](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-request.md)                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmWalletSelfServiceResourceGetTransactionsResponse](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |