# Connector

The payment integration connector type

## Example Usage

```typescript
import { Connector } from "crm/models/operations";

let value: Connector = "PLUGIN";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"MIXPANEL" | "MONGO" | "MAILCHIMP" | "STRIPE" | "SMTP" | "TWILIO" | "SMPP" | "BRAINTREE" | "FIREBASE" | "JCC" | "JCC_MERCHANT" | "GOOGLEPLACES" | "WHATSAPP" | "SETTLE" | "UNIFI" | "TWINSOFT" | "ALOHA" | "PLUGIN" | Unrecognized<string>
```