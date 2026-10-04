# UpsellPriceModel

The pricing model:
 * `FLAT`
 * `TIERED`
 * `VOLUME`
 * `STAIRSTEP`

## Example Usage

```typescript
import { UpsellPriceModel } from "crm/models/operations";

let value: UpsellPriceModel = "FLAT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```