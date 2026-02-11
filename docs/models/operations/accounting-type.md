# AccountingType

Defines the accounting type of the settlement transaction

## Example Usage

```typescript
import { AccountingType } from "crm/models/operations";

let value: AccountingType = "DEBIT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DEBIT" | "CREDIT" | Unrecognized<string>
```