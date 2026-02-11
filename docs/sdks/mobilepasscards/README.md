# MobilePassCards

## Overview

All Api’s associated to Mobile Pass Cards

### Available Operations

* [comCrmWalletPassesSelfServiceResourceGetAndroidWalletPass](#comcrmwalletpassesselfserviceresourcegetandroidwalletpass) - Get Android Wallet Pass
* [comCrmWalletPassesSelfServiceResourceGetApplePass](#comcrmwalletpassesselfserviceresourcegetapplepass) - Get Apple Pass
* [comCrmWalletPassesSelfServiceResourceGetGooglePass](#comcrmwalletpassesselfserviceresourcegetgooglepass) - Get Google Pass

## comCrmWalletPassesSelfServiceResourceGetAndroidWalletPass

Retrieves a contact's mobile pass card for an alternative Android wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletPassesSelfServiceResource_getAndroidWalletPass" method="get" path="/self-service/v2/android_wallet_pass/{organisationId}/contacts/{contactId}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.mobilePassCards.comCrmWalletPassesSelfServiceResourceGetAndroidWalletPass({
    contactId: "<id>",
    organisationId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { mobilePassCardsComCrmWalletPassesSelfServiceResourceGetAndroidWalletPass } from "crm/funcs/mobile-pass-cards-com-crm-wallet-passes-self-service-resource-get-android-wallet-pass.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await mobilePassCardsComCrmWalletPassesSelfServiceResourceGetAndroidWalletPass(crm, {
    contactId: "<id>",
    organisationId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("mobilePassCardsComCrmWalletPassesSelfServiceResourceGetAndroidWalletPass failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                             | Type                                                                                                                                                                                  | Required                                                                                                                                                                              | Description                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `request`                                                                                                                                                                             | [operations.ComCrmWalletPassesSelfServiceResourceGetAndroidWalletPassRequest](../../models/operations/com-crm-wallet-passes-self-service-resource-get-android-wallet-pass-request.md) | :heavy_check_mark:                                                                                                                                                                    | The request object to use for the request.                                                                                                                                            |
| `options`                                                                                                                                                                             | RequestOptions                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                    | Used to set various options for making HTTP requests.                                                                                                                                 |
| `options.fetchOptions`                                                                                                                                                                | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                               | :heavy_minus_sign:                                                                                                                                                                    | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed.        |
| `options.retries`                                                                                                                                                                     | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                    | Enables retrying HTTP requests under certain failure conditions.                                                                                                                      |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletPassesSelfServiceResourceGetApplePass

Retrieves a mobile pass card for an Apple wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletPassesSelfServiceResource_getApplePass" method="get" path="/self-service/v2/apple_pass/{organisationId}/contacts/{contactId}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.mobilePassCards.comCrmWalletPassesSelfServiceResourceGetApplePass({
    contactId: "<id>",
    organisationId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { mobilePassCardsComCrmWalletPassesSelfServiceResourceGetApplePass } from "crm/funcs/mobile-pass-cards-com-crm-wallet-passes-self-service-resource-get-apple-pass.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await mobilePassCardsComCrmWalletPassesSelfServiceResourceGetApplePass(crm, {
    contactId: "<id>",
    organisationId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("mobilePassCardsComCrmWalletPassesSelfServiceResourceGetApplePass failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletPassesSelfServiceResourceGetApplePassRequest](../../models/operations/com-crm-wallet-passes-self-service-resource-get-apple-pass-request.md)           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmWalletPassesSelfServiceResourceGetGooglePass

Retrieves a mobile pass card for a Google wallet.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.WalletPassesSelfServiceResource_getGooglePass" method="get" path="/self-service/v2/google_pass/{organisationId}/contacts/{contactId}" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.mobilePassCards.comCrmWalletPassesSelfServiceResourceGetGooglePass({
    contactId: "<id>",
    organisationId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { mobilePassCardsComCrmWalletPassesSelfServiceResourceGetGooglePass } from "crm/funcs/mobile-pass-cards-com-crm-wallet-passes-self-service-resource-get-google-pass.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await mobilePassCardsComCrmWalletPassesSelfServiceResourceGetGooglePass(crm, {
    contactId: "<id>",
    organisationId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("mobilePassCardsComCrmWalletPassesSelfServiceResourceGetGooglePass failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmWalletPassesSelfServiceResourceGetGooglePassRequest](../../models/operations/com-crm-wallet-passes-self-service-resource-get-google-pass-request.md)         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |