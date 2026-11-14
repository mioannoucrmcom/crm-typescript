# FeeType

Defines the fee type
 * `CONTRIBUTION` - Contribution fee, applied on award transactions
 * `SETTLEMENT` - Settlement fee, applied on award/spend transactions


## Example Usage

```typescript
import { FeeType } from "crm/models/operations";

let value: FeeType = "CONTRIBUTION";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"CONTRIBUTION" | "SETTLEMENT" | Unrecognized<string>
```