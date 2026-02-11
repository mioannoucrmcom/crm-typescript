# CrossSellPriceModel

The pricing model:
 * `FLAT`
 * `TIERED`
 * `VOLUME`
 * `STAIRSTEP`

## Example Usage

```typescript
import { CrossSellPriceModel } from "crm/models/operations";

let value: CrossSellPriceModel = "VOLUME";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```