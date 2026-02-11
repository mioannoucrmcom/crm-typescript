# ComponentProductPriceModel

Price model

## Example Usage

```typescript
import { ComponentProductPriceModel } from "crmcom/models/operations";

let value: ComponentProductPriceModel = "STAIRSTEP";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```