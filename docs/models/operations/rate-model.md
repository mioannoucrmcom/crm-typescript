# RateModel

the rate model of price

## Example Usage

```typescript
import { RateModel } from "crm/models/operations";

let value: RateModel = "FLAT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```