# ComCrmServiceRequestSelfServiceResourceCreateServiceRequestFileRequestBody

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceCreateServiceRequestFileRequestBody } from "crmcom/models/operations";

let value:
  ComCrmServiceRequestSelfServiceResourceCreateServiceRequestFileRequestBody = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    fileId: "30526723-24a3-e4e3-1a75-b26b1b41f05c",
    link:
      "https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug",
    description: "PowerPoint demo",
  };
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          | Example                                                                                              |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `id`                                                                                                 | *string*                                                                                             | :heavy_minus_sign:                                                                                   | The entity identifier that will be created                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                 |
| `fileId`                                                                                             | *string*                                                                                             | :heavy_check_mark:                                                                                   | The file (identifier) to be connected. You must provide either a file_id or a link                   | 30526723-24a3-e4e3-1a75-b26b1b41f05c                                                                 |
| `link`                                                                                               | *string*                                                                                             | :heavy_check_mark:                                                                                   | The URL endpoint to be attached (either file_id or link must be provided)                            | https://crmcom.sharepoint.com/:x:/s/servicerequests/EZx2qopbvfN3uj1o3dOqbPm52Ct6bg?rtime=w0ic-hfG2Ug |
| `description`                                                                                        | *string*                                                                                             | :heavy_minus_sign:                                                                                   | The file description                                                                                 | PowerPoint demo                                                                                      |