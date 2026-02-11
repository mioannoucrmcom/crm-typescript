# UpsellTaxModel

Defines whether the price is tax inclusive or not. Defaults to the system's Taxation setting

## Example Usage

```typescript
import { UpsellTaxModel } from "crm/models/operations";

let value: UpsellTaxModel = "TAX_INCLUSIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"TAX_INCLUSIVE" | "TAX_EXCLUSIVE" | Unrecognized<string>
```