# ComCrmApplicationSelfServiceResourceGetApplicationContent

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationContent } from "crm/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationContent = {
  url: "https?/crm.com",
  richContent: "Terms & Conditions",
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               | Example                                                                   |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `type`                                                                    | [operations.InformationType](../../models/operations/information-type.md) | :heavy_minus_sign:                                                        | The content type                                                          |                                                                           |
| `url`                                                                     | *string*                                                                  | :heavy_minus_sign:                                                        | The detail URL endpoint (URL or Content is required)                      | https?/crm.com                                                            |
| `richContent`                                                             | *string*                                                                  | :heavy_minus_sign:                                                        | The detail rich content (URL or Content is required)                      | Terms & Conditions                                                        |