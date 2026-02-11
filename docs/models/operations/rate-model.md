# RateModel

the rate model of price

## Example Usage

```typescript
import { RateModel } from "crm/models/operations";

let value: RateModel = "FLAT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```