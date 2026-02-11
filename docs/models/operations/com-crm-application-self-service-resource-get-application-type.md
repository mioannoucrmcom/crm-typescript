# ComCrmApplicationSelfServiceResourceGetApplicationType

The application type:
 * `NATIVE` - Mobile Consumer Applications (Apple and Google)
 * `NATIVE_MERCHANT` - Mobile Merchant Applications (Apple and Google)
 * `WEB` - Web Portal
 * `CAPTIVE` - Captive Portal
 * `CONSUMER_APP` - Consumer App (Portal and App)


## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationType } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationType = "CAPTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"NATIVE" | "NATIVE_MERCHANT" | "WEB" | "CAPTIVE" | "CONSUMER_APP" | Unrecognized<string>
```