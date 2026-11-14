# Model

Defines the consumer ordering model

## Example Usage

```typescript
import { Model } from "crm/models/operations";

let value: Model = "SINGLE_BUSINESS";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"MARKETPLACE" | "SINGLE_BUSINESS" | Unrecognized<string>
```