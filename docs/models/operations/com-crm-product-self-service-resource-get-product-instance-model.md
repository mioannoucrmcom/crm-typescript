# ComCrmProductSelfServiceResourceGetProductInstanceModel

Determines whether a service is managed as a single quantity or as separate, independently managed instances on a subscription

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductInstanceModel } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductInstanceModel =
  "QUANTITY_BASED";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"QUANTITY_BASED" | "LINE_BASED" | Unrecognized<string>
```