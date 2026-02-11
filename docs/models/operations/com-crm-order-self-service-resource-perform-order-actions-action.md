# ComCrmOrderSelfServiceResourcePerformOrderActionsAction

Defines the new life cycle state of the Order. Used to start the progress of an order, complete it or cancel it

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourcePerformOrderActionsAction } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourcePerformOrderActionsAction =
  "MARK_FAVORITE";
```

## Values

```typescript
"START_PROGRESS" | "COMPLETE" | "CANCEL" | "MARK_FAVORITE" | "PRINT_ORDER" | "ORDER_PROVISION"
```