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
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```