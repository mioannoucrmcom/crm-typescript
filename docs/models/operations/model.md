# Model

Defines the consumer ordering model

## Example Usage

```typescript
import { Model } from "crm/models/operations";

let value: Model = "SINGLE_BUSINESS";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"MARKETPLACE" | "SINGLE_BUSINESS" | Unrecognized<string>
```