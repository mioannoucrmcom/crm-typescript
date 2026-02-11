# SelfSubmitMethod

## Example Usage

```typescript
import { SelfSubmitMethod } from "crm/models/operations";

let value: SelfSubmitMethod = "BARCODE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BARCODE" | "TRX_CODE" | Unrecognized<string>
```