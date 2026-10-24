# ComCrmApplicationSelfServiceResourceGetApplicationType

The application type:
 * `NATIVE` - Mobile Consumer Applications (Apple and Google)
 * `NATIVE_MERCHANT` - Mobile Merchant Applications (Apple and Google)
 * `WEB` - Web Portal
 * `CAPTIVE` - Captive Portal
 * `CONSUMER_APP` - Consumer App (Portal and App)


## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationType } from "crm/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationType = "CAPTIVE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"NATIVE" | "NATIVE_MERCHANT" | "WEB" | "CAPTIVE" | "CONSUMER_APP" | Unrecognized<string>
```