# ShortcutType

Shortcuts valid types (for front-end applications)

## Example Usage

```typescript
import { ShortcutType } from "crmcom/models/operations";

let value: ShortcutType = "TOP_UP_WALLET";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"CONTACT_CODE" | "LOCATIONS" | "OTP_TO_SPEND" | "RECLAIM_PURCHASE" | "TOP_UP_WALLET" | "REFER_A_FRIEND" | "SERVICE_REQUEST" | "REDEEM_A_PASS" | "REQUEST_MONEY" | "SEND_MONEY" | "COMMUNITIES" | "ORDER" | "DONATE" | "ELECTRONIC_GIFT_PASS" | Unrecognized<string>
```