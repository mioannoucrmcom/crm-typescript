# ComCrmApplicationSelfServiceResourceGetApplicationCodeFormat

The alternative token code format. This code can be in the form of a barcode or QR code

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationCodeFormat } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationCodeFormat =
  "BARCODE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BARCODE" | "QR_CODE" | Unrecognized<string>
```