# TransferEntity

## Example Usage

```typescript
import { TransferEntity } from "crm/models/operations";

let value: TransferEntity = "WALLET";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ACCOUNT" | "WALLET" | Unrecognized<string>
```