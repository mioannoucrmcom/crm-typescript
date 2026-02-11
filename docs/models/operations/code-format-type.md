# CodeFormatType

The pass code type to be used

## Example Usage

```typescript
import { CodeFormatType } from "crmcom/models/operations";

let value: CodeFormatType = "ALPHANUMERIC";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ALPHANUMERIC" | "ALPHABETIC" | "NUMERIC" | Unrecognized<string>
```