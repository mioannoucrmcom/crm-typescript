# SignUpMethod

Defines how closed loop (controlled) sign ups will be validated against, like specific email domain (required only if sign up option is controlled based sign up)

## Example Usage

```typescript
import { SignUpMethod } from "crm/models/operations";

let value: SignUpMethod = "CODE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"EMAIL_DOMAIN" | "CODE" | Unrecognized<string>
```