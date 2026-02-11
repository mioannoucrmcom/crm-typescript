# WalletCodeFormat

The contact's wallet code is used to uniquely identify them on front-end devices. This code can be in the form of a barcode or QR code

## Example Usage

```typescript
import { WalletCodeFormat } from "crm/models/operations";

let value: WalletCodeFormat = "BARCODE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"BARCODE" | "QR_CODE" | Unrecognized<string>
```