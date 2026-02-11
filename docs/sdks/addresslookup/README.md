# AddressLookup

## Overview

Address Lookup

### Available Operations

* [comCrmAddressRegistrySelfServiceResourceList](#comcrmaddressregistryselfserviceresourcelist) - Search Addresses
* [comCrmAddressRegistrySelfServiceResourceGetAddress](#comcrmaddressregistryselfserviceresourcegetaddress) - Get Address

## comCrmAddressRegistrySelfServiceResourceList

Returns a list of addresses based on the Google Place Autocomplete API. A retrieved google place id can then be used for the Get Address API. A version 4 UUID should be used as the session_id for a given session. A session starts with one or more Search Addresses API calls, and ends with one Get Address API call. Make sure to generate a new session_id for each new session. When a session_id is reused after the session has concluded, Per Request billing applies instead of Per Session billing.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AddressRegistrySelfServiceResource_list" method="get" path="/self-service/v2/addresses" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crmcom.addressLookup.comCrmAddressRegistrySelfServiceResourceList({
    countries: "FR,US",
    input: "Elia Papakyriakou 21",
    sessionId: "b9a5d80f-f2fa-4f62-b29f-9d288186bdf1",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { addressLookupComCrmAddressRegistrySelfServiceResourceList } from "crmcom/funcs/address-lookup-com-crm-address-registry-self-service-resource-list.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await addressLookupComCrmAddressRegistrySelfServiceResourceList(crmcom, {
    countries: "FR,US",
    input: "Elia Papakyriakou 21",
    sessionId: "b9a5d80f-f2fa-4f62-b29f-9d288186bdf1",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("addressLookupComCrmAddressRegistrySelfServiceResourceList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAddressRegistrySelfServiceResourceListRequest](../../models/operations/com-crm-address-registry-self-service-resource-list-request.md)                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAddressRegistrySelfServiceResourceListResponse](../../models/operations/com-crm-address-registry-self-service-resource-list-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmAddressRegistrySelfServiceResourceGetAddress

Returns address details based on the Google Place Details API. The google place id used for this API could be retrieved with the Search Addresses API. A version 4 UUID should be used as the session_id for a given session. A session starts with one or more Search Addresses API calls, and ends with one Get Address API call. Make sure to generate a new session_id for each new session. When a session_id is reused after the session has concluded, Per Request billing applies instead of Per Session billing.

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.AddressRegistrySelfServiceResource_getAddress" method="get" path="/self-service/v2/get_addresses" example="Example 1" -->
```typescript
import { Crmcom } from "crmcom";

const crmcom = new Crmcom();

async function run() {
  const result = await crmcom.addressLookup.comCrmAddressRegistrySelfServiceResourceGetAddress({
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    googlePlaceId: "ChIJLU7jZClu5kcR4PcOOO6p3I0",
    latlng: "<value>",
    sessionId: "b9a5d80f-f2fa-4f62-b29f-9d288186bdf1",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmcomCore } from "crmcom/core.js";
import { addressLookupComCrmAddressRegistrySelfServiceResourceGetAddress } from "crmcom/funcs/address-lookup-com-crm-address-registry-self-service-resource-get-address.js";

// Use `CrmcomCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crmcom = new CrmcomCore();

async function run() {
  const res = await addressLookupComCrmAddressRegistrySelfServiceResourceGetAddress(crmcom, {
    secretAPIKey: process.env["CRM_SECRET_API_KEY"] ?? "",
  }, {
    googlePlaceId: "ChIJLU7jZClu5kcR4PcOOO6p3I0",
    latlng: "<value>",
    sessionId: "b9a5d80f-f2fa-4f62-b29f-9d288186bdf1",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("addressLookupComCrmAddressRegistrySelfServiceResourceGetAddress failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmAddressRegistrySelfServiceResourceGetAddressRequest](../../models/operations/com-crm-address-registry-self-service-resource-get-address-request.md)          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `security`                                                                                                                                                                     | [operations.ComCrmAddressRegistrySelfServiceResourceGetAddressSecurity](../../models/operations/com-crm-address-registry-self-service-resource-get-address-security.md)        | :heavy_check_mark:                                                                                                                                                             | The security requirements to use for the request.                                                                                                                              |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmAddressRegistrySelfServiceResourceGetAddressResponse](../../models/operations/com-crm-address-registry-self-service-resource-get-address-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |