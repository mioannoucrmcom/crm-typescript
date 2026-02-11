# TransferRestriction

## Example Usage

```typescript
import { TransferRestriction } from "crm/models/operations";

let value: TransferRestriction = "OPEN";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"OPEN" | "COMMERCE" | Unrecognized<string>
```