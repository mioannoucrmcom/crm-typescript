# Sso

Support contacts authentication using an Open ID Connect provider (that enables single-sign-on)

## Example Usage

```typescript
import { Sso } from "crm/models/operations";

let value: Sso = {
  isSupported: true,
};
```

## Fields

| Field                                              | Type                                               | Required                                           | Description                                        | Example                                            |
| -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- |
| `isSupported`                                      | *boolean*                                          | :heavy_minus_sign:                                 | Defines whether OpenID connect is supported or not | true                                               |