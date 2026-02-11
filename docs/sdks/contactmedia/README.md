# ContactMedia

## Overview

Contact Media APIs

### Available Operations

* [comCrmContactSelfServiceMediaResourceSign](#comcrmcontactselfservicemediaresourcesign) - Create a Self Service V2 Media Upload Signature

## comCrmContactSelfServiceMediaResourceSign

Create a Self Service V2 Media Upload Signature

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceMediaResource_sign" method="post" path="/self-service/v2/media/upload/signature" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactMedia.comCrmContactSelfServiceMediaResourceSign({
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactMediaComCrmContactSelfServiceMediaResourceSign } from "crm/funcs/contact-media-com-crm-contact-self-service-media-resource-sign.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactMediaComCrmContactSelfServiceMediaResourceSign(crm, {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactMediaComCrmContactSelfServiceMediaResourceSign failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceMediaResourceSignRequest](../../models/operations/com-crm-contact-self-service-media-resource-sign-request.md)                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |