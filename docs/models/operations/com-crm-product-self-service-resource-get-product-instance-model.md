# ComCrmProductSelfServiceResourceGetProductInstanceModel

Determines whether a service is managed as a single quantity or as separate, independently managed instances on a subscription

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductInstanceModel } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductInstanceModel =
  "QUANTITY_BASED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"QUANTITY_BASED" | "LINE_BASED" | Unrecognized<string>
```