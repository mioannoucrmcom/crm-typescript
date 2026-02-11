# Code

The command (unique) code. Its value varies according to the implemented IRD commands per provisioning provider.

## Example Usage

```typescript
import { Code } from "crmcom/models/operations";

let value: Code = "REFRESH";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"REFRESH" | "RESET_PIN" | Unrecognized<string>
```