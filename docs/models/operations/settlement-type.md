# SettlementType

Defines the settlement transaction type
 * `AWARD` - Award Transaction
 * `SPEND` - Spend Transaction
 * `AWARD_FEE` - Award Settlement Fee
 * `SPEND_FEE` - Spend Settlement Fee


## Example Usage

```typescript
import { SettlementType } from "crm/models/operations";

let value: SettlementType = "AWARD";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AWARD" | "SPEND" | "AWARD_FEE" | "SPEND_FEE" | Unrecognized<string>
```