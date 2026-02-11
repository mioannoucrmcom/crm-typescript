# PricePriceModel

Price model of the price

## Example Usage

```typescript
import { PricePriceModel } from "crmcom/models/operations";

let value: PricePriceModel = "TIERED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```