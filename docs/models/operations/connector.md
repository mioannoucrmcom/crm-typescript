# Connector

The payment integration connector type

## Example Usage

```typescript
import { Connector } from "crm/models/operations";

let value: Connector = "PLUGIN";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"MIXPANEL" | "MONGO" | "MAILCHIMP" | "STRIPE" | "SMTP" | "TWILIO" | "SMPP" | "BRAINTREE" | "FIREBASE" | "JCC" | "JCC_MERCHANT" | "GOOGLEPLACES" | "WHATSAPP" | "SETTLE" | "UNIFI" | "TWINSOFT" | "ALOHA" | "PLUGIN" | Unrecognized<string>
```