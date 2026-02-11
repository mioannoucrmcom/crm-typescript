# ComponentPricePriceModel

Price model

## Example Usage

```typescript
import { ComponentPricePriceModel } from "crm/models/operations";

let value: ComponentPricePriceModel = "FLAT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"FLAT" | "TIERED" | "VOLUME" | "STAIRSTEP" | Unrecognized<string>
```