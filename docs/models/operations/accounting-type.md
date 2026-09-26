# AccountingType

Defines the accounting type of the settlement transaction

## Example Usage

```typescript
import { AccountingType } from "crm/models/operations";

let value: AccountingType = "DEBIT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"DEBIT" | "CREDIT" | Unrecognized<string>
```