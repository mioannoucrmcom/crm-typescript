# DeliveryTimeSelection

Defines how the contact selects the delivery time for their order: explicit_delivery_time allows the contact to choose a specific date and time, slot_selection allows them to select from available time slots, and no_time means the delivery date and time are determined by the organisation.

## Example Usage

```typescript
import { DeliveryTimeSelection } from "crmcom/models/operations";

let value: DeliveryTimeSelection = "NO_TIME";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"EXPLICIT_DELIVERY_TIME" | "SLOT_SELECTION" | "NO_TIME" | Unrecognized<string>
```