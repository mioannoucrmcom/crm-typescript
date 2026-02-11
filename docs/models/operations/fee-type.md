# FeeType

Defines the fee type
 * `CONTRIBUTION` - Contribution fee, applied on award transactions
 * `SETTLEMENT` - Settlement fee, applied on award/spend transactions


## Example Usage

```typescript
import { FeeType } from "crmcom/models/operations";

let value: FeeType = "CONTRIBUTION";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"CONTRIBUTION" | "SETTLEMENT" | Unrecognized<string>
```