# ContactPaymentMethods

## Overview

Contact Payment Methods

### Available Operations

* [comCrmContactSelfServiceResourceGetPaymentMethods](#comcrmcontactselfserviceresourcegetpaymentmethods) - List Payment Methods
* [comCrmContactSelfServiceResourceAddPaymentMethod](#comcrmcontactselfserviceresourceaddpaymentmethod) - Add Payment Method
* [comCrmContactSelfServiceResourceUpdatePaymentMethod](#comcrmcontactselfserviceresourceupdatepaymentmethod) - Update Payment Method
* [comCrmContactSelfServiceResourceDeletePaymentMethod](#comcrmcontactselfserviceresourcedeletepaymentmethod) - Remove Payment Method

## comCrmContactSelfServiceResourceGetPaymentMethods

List of Payment methods allocated to contact.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_getPaymentMethods" method="get" path="/self-service/v2/contacts/{id}/payment_methods" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactPaymentMethods.comCrmContactSelfServiceResourceGetPaymentMethods({
    id: "<id>",
    classification: "WALLET",
    financialTypes: "Allowed values:\r\nPAYMENTS\r\nPAYOUTS\r\nREFUNDS\r\nTOP_UPS",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactPaymentMethodsComCrmContactSelfServiceResourceGetPaymentMethods } from "crmcom/funcs/contact-payment-methods-com-crm-contact-self-service-resource-get-payment-methods.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactPaymentMethodsComCrmContactSelfServiceResourceGetPaymentMethods(crmcom, {
    id: "<id>",
    classification: "WALLET",
    financialTypes: "Allowed values:\r\nPAYMENTS\r\nPAYOUTS\r\nREFUNDS\r\nTOP_UPS",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactPaymentMethodsComCrmContactSelfServiceResourceGetPaymentMethods failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsRequest](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-request.md)            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceGetPaymentMethodsResponse](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceAddPaymentMethod

Add a new payment method for a contact supports Card, Account Debits and Wallet payment methods</br></br><h4>Notes</h4>
                                    <div class="description spec-item-section__description"><p><em><strong>JCC Merchant Gateway</strong></em></p>
<ul>
<li>Perform <a href="#fingerprint" class="link-internal link-method" target="_self">Fingerprint</a> to retrieve the card masked &amp; hashed numbers and the country of issue</li>
<li>Set the retrieved masked number, hashed number and country of issue on the related “card” collection</li>
</ul>
<p><em><strong>Settle Gateway</strong></em></p>
<ul>
<li>Set the phone country code, phone number and msisdn (phone country + number) on the related “phone” collection</li>
</ul>

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_addPaymentMethod" method="post" path="/self-service/v2/contacts/{id}/payment_methods" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactPaymentMethods.comCrmContactSelfServiceResourceAddPaymentMethod({
    id: "<id>",
    body: {
      name: "PayPal",
      isPrimary: true,
      paymentMethodType: "CARD",
      notes: "Lorem Ipsum",
      card: {
        name: "Default Card",
        first6: "424242",
        last4: "4242",
        brand: "VISA",
        expirationMonth: 2,
        expirationYear: 2020,
        countryOfIssue: "CYP",
        cardHolderDetails: {
          cardHolderName: "John Alias Doe",
          addressLine1: "Elia Papakyriakou",
          addressLine2: "Tower Stars",
          addressCity: "Nicosia",
          addressZip: "2000",
          addressState: "Egkomi",
          addressCountry: "CYP",
          useBillingAddress: true,
        },
        gatewayToken: [
          {
            gateway: "JCC",
            token: "",
            integrationId: "",
          },
        ],
      },
      wallet: {
        phoneDetails: {
          name: "Primary phone",
          countryCode: "CYP",
          number: "91000000",
          msisdn: "35791000000",
        },
        email: "",
        gatewayToken: [
          {
            gateway: "SETTLE",
            token: "",
            integrationId: "",
          },
        ],
      },
      accountDebit: {
        accountName: "",
        accountNumber: "001002001",
        iban: "SE3550000000054910000003",
        sortCode: "",
        bank: "Barclays",
        bankCode: "102491",
        branch: "Ascot",
        swift: "12345678",
        accountType: "SAVINGS",
        mandate: {
          signDate: 1,
        },
        gatewayToken: [
          {
            gateway: "JCC_MERCHANT",
            token: "",
            integrationId: "",
          },
        ],
        accountHolderDetails: {
          accountHolderName: "",
          addressLine1: "",
          addressLine2: "",
          addressCity: "",
          addressZip: "",
          addressState: "",
          addressCountry: "CYP",
          useBillingAddress: true,
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
import { CrmcomCore } from "crmcom/core.js";
import { contactPaymentMethodsComCrmContactSelfServiceResourceAddPaymentMethod } from "crmcom/funcs/contact-payment-methods-com-crm-contact-self-service-resource-add-payment-method.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactPaymentMethodsComCrmContactSelfServiceResourceAddPaymentMethod(crmcom, {
    id: "<id>",
    body: {
      name: "PayPal",
      isPrimary: true,
      paymentMethodType: "CARD",
      notes: "Lorem Ipsum",
      card: {
        name: "Default Card",
        first6: "424242",
        last4: "4242",
        brand: "VISA",
        expirationMonth: 2,
        expirationYear: 2020,
        countryOfIssue: "CYP",
        cardHolderDetails: {
          cardHolderName: "John Alias Doe",
          addressLine1: "Elia Papakyriakou",
          addressLine2: "Tower Stars",
          addressCity: "Nicosia",
          addressZip: "2000",
          addressState: "Egkomi",
          addressCountry: "CYP",
          useBillingAddress: true,
        },
        gatewayToken: [
          {
            gateway: "JCC",
            token: "",
            integrationId: "",
          },
        ],
      },
      wallet: {
        phoneDetails: {
          name: "Primary phone",
          countryCode: "CYP",
          number: "91000000",
          msisdn: "35791000000",
        },
        email: "",
        gatewayToken: [
          {
            gateway: "SETTLE",
            token: "",
            integrationId: "",
          },
        ],
      },
      accountDebit: {
        accountName: "",
        accountNumber: "001002001",
        iban: "SE3550000000054910000003",
        sortCode: "",
        bank: "Barclays",
        bankCode: "102491",
        branch: "Ascot",
        swift: "12345678",
        accountType: "SAVINGS",
        mandate: {
          signDate: 1,
        },
        gatewayToken: [
          {
            gateway: "JCC_MERCHANT",
            token: "",
            integrationId: "",
          },
        ],
        accountHolderDetails: {
          accountHolderName: "",
          addressLine1: "",
          addressLine2: "",
          addressCity: "",
          addressZip: "",
          addressState: "",
          addressCountry: "CYP",
          useBillingAddress: true,
        },
      },
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactPaymentMethodsComCrmContactSelfServiceResourceAddPaymentMethod failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodRequest](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-request.md)              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceAddPaymentMethodResponse](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceUpdatePaymentMethod

Update an existing payment method for a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_updatePaymentMethod" method="put" path="/self-service/v2/contacts/{id}/payment_methods/{payment_method_id}" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.contactPaymentMethods.comCrmContactSelfServiceResourceUpdatePaymentMethod({
    id: "<id>",
    paymentMethodId: "<id>",
    body: {
      name: "",
      isPrimary: true,
      notes: "Lorem Ipsum",
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
import { contactPaymentMethodsComCrmContactSelfServiceResourceUpdatePaymentMethod } from "crmcom/funcs/contact-payment-methods-com-crm-contact-self-service-resource-update-payment-method.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactPaymentMethodsComCrmContactSelfServiceResourceUpdatePaymentMethod(crmcom, {
    id: "<id>",
    paymentMethodId: "<id>",
    body: {
      name: "",
      isPrimary: true,
      notes: "Lorem Ipsum",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactPaymentMethodsComCrmContactSelfServiceResourceUpdatePaymentMethod failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceUpdatePaymentMethodRequest](../../models/operations/com-crm-contact-self-service-resource-update-payment-method-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceUpdatePaymentMethodResponse](../../models/operations/com-crm-contact-self-service-resource-update-payment-method-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceDeletePaymentMethod

Remove an existing payment method from a specific contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_deletePaymentMethod" method="delete" path="/self-service/v2/contacts/{id}/payment_methods/{payment_method_id}" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crmcom.contactPaymentMethods.comCrmContactSelfServiceResourceDeletePaymentMethod({
    id: "<id>",
    paymentMethodId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { contactPaymentMethodsComCrmContactSelfServiceResourceDeletePaymentMethod } from "crmcom/funcs/contact-payment-methods-com-crm-contact-self-service-resource-delete-payment-method.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactPaymentMethodsComCrmContactSelfServiceResourceDeletePaymentMethod(crmcom, {
    id: "<id>",
    paymentMethodId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactPaymentMethodsComCrmContactSelfServiceResourceDeletePaymentMethod failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceDeletePaymentMethodRequest](../../models/operations/com-crm-contact-self-service-resource-delete-payment-method-request.md)        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |