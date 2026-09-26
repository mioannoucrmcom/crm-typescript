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

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```