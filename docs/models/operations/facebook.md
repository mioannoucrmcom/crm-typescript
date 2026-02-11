# Facebook

Defines whether contacts can register & sign-in based on Facebook (including Facebook authentication details)

## Example Usage

```typescript
import { Facebook } from "crm/models/operations";

let value: Facebook = {
  isSupported: true,
  appId: "sfsdf-23-we-wer-3ew-dw",
};
```

## Fields

| Field                                                     | Type                                                      | Required                                                  | Description                                               | Example                                                   |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `isSupported`                                             | *boolean*                                                 | :heavy_minus_sign:                                        | Defines whether Facebook authentication is enabled or not | true                                                      |
| `appId`                                                   | *string*                                                  | :heavy_minus_sign:                                        | Facebook App ID required for FB authentication            | sfsdf-23-we-wer-3ew-dw                                    |