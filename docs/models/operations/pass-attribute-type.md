# PassAttributeType

The pass supplementary attribute type

## Example Usage

```typescript
import { PassAttributeType } from "crmcom/models/operations";

let value: PassAttributeType = "CODE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"CODE" | "PIN" | Unrecognized<string>
```