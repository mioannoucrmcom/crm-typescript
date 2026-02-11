# ComCrmContactSelfServiceResourceGetFilesContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetFilesContent } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetFilesContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  file: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
    mime: "DOC",
  },
  description: "Screenshot sent by customer",
  link:
    "https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                | Example                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                       | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The entity identifier                                                                                                                      | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                       |
| `file`                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceGetFilesFile](../../models/operations/com-crm-contact-self-service-resource-get-files-file.md) | :heavy_minus_sign:                                                                                                                         | The attached file details                                                                                                                  |                                                                                                                                            |
| `description`                                                                                                                              | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The attachment description                                                                                                                 | Screenshot sent by customer                                                                                                                |
| `link`                                                                                                                                     | *string*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The attached URL endpoint                                                                                                                  | https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug                                       |