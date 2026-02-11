# ContactImages

## Overview

Contact Images

### Available Operations

* [comCrmContactSelfServiceResourceUploadImage](#comcrmcontactselfserviceresourceuploadimage) - Upload Image
* [comCrmContactSelfServiceResourceDeleteImage](#comcrmcontactselfserviceresourcedeleteimage) - Delete Contact Image

## comCrmContactSelfServiceResourceUploadImage

Upload image for a contact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_uploadImage" method="put" path="/self-service/v2/contacts/{id}/image" example="Example 1" -->
```typescript
import { Crm } from "crm";
import { openAsBlob } from "node:fs";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const result = await crm.contactImages.comCrmContactSelfServiceResourceUploadImage({
    id: "<id>",
    body: {
      image: await openAsBlob("example.file"),
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
import { contactImagesComCrmContactSelfServiceResourceUploadImage } from "crm/funcs/contact-images-com-crm-contact-self-service-resource-upload-image.js";
import { openAsBlob } from "node:fs";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactImagesComCrmContactSelfServiceResourceUploadImage(crm, {
    id: "<id>",
    body: {
      image: await openAsBlob("example.file"),
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("contactImagesComCrmContactSelfServiceResourceUploadImage failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceUploadImageRequest](../../models/operations/com-crm-contact-self-service-resource-upload-image-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.ComCrmContactSelfServiceResourceUploadImageResponse](../../models/operations/com-crm-contact-self-service-resource-upload-image-response.md)\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |

## comCrmContactSelfServiceResourceDeleteImage

Delete the contact image

### Example Usage

<!-- UsageSnippet language="typescript" operationID="com.crm.ContactSelfServiceResource_deleteImage" method="delete" path="/self-service/v2/contacts/{id}/image" -->
```typescript
import { Crm } from "crm";

const crm = new Crm({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  await crm.contactImages.comCrmContactSelfServiceResourceDeleteImage({
    id: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { CrmCore } from "crm/core.js";
import { contactImagesComCrmContactSelfServiceResourceDeleteImage } from "crm/funcs/contact-images-com-crm-contact-self-service-resource-delete-image.js";

// Use `CrmCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const crm = new CrmCore({
  authorizationSelfService: process.env["CRM_AUTHORIZATION_SELF_SERVICE"] ?? "",
});

async function run() {
  const res = await contactImagesComCrmContactSelfServiceResourceDeleteImage(crm, {
    id: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("contactImagesComCrmContactSelfServiceResourceDeleteImage failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceDeleteImageRequest](../../models/operations/com-crm-contact-self-service-resource-delete-image-request.md)                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type             | Status Code            | Content Type           |
| ---------------------- | ---------------------- | ---------------------- |
| errors.CrmDefaultError | 4XX, 5XX               | \*/\*                  |