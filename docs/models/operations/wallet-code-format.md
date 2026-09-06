# WalletCodeFormat

The contact's wallet code is used to uniquely identify them on front-end devices. This code can be in the form of a barcode or QR code

## Example Usage

```typescript
import { WalletCodeFormat } from "crm/models/operations";

let value: WalletCodeFormat = "BARCODE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"BARCODE" | "QR_CODE" | Unrecognized<string>
```