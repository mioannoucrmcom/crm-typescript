# ComCrmContactSelfServiceResourceGetFilesResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetFilesResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetFilesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      file: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
        mime: "DOC",
      },
      description: "Screenshot sent by customer",
      link:
        "https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
    },
  ],
};
```

## Fields

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceGetFilesPaging](../../models/operations/com-crm-contact-self-service-resource-get-files-paging.md)     | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |
| `content`                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceGetFilesContent](../../models/operations/com-crm-contact-self-service-resource-get-files-content.md)[] | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |