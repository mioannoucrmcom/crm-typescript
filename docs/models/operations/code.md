# Code

The command (unique) code. Its value varies according to the implemented IRD commands per provisioning provider.

## Example Usage

```typescript
import { Code } from "crm/models/operations";

let value: Code = "REFRESH";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"REFRESH" | "RESET_PIN" | Unrecognized<string>
```