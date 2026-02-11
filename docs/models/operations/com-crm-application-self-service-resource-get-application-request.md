# ComCrmApplicationSelfServiceResourceGetApplicationRequest

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationRequest } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationRequest = {
  cloudName: "crm",
  platformAppId: "f9e4b742-bfe1-09dc-f623-de71aaed61ff",
  version: "\"1.1\"",
};
```

## Fields

| Field                                        | Type                                         | Required                                     | Description                                  | Example                                      |
| -------------------------------------------- | -------------------------------------------- | -------------------------------------------- | -------------------------------------------- | -------------------------------------------- |
| `cloudName`                                  | *string*                                     | :heavy_minus_sign:                           | Use cloud name to retrieve Web APP settings. | crm                                          |
| `platformAppId`                              | *string*                                     | :heavy_check_mark:                           | The platform application identifier          | f9e4b742-bfe1-09dc-f623-de71aaed61ff         |
| `version`                                    | *string*                                     | :heavy_minus_sign:                           | The application version number               | "1.1"                                        |