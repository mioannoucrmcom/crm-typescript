# Multitenancy

Defines whether multitenancy features will be available

## Example Usage

```typescript
import { Multitenancy } from "crm/models/operations";

let value: Multitenancy = {
  isSupported: true,
};
```

## Fields

| Field                                     | Type                                      | Required                                  | Description                               | Example                                   |
| ----------------------------------------- | ----------------------------------------- | ----------------------------------------- | ----------------------------------------- | ----------------------------------------- |
| `isSupported`                             | *boolean*                                 | :heavy_minus_sign:                        | Defines whether multitenancy is supported | true                                      |