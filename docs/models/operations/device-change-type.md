# DeviceChangeType

## Example Usage

```typescript
import { DeviceChangeType } from "crmcom/models/operations";

let value: DeviceChangeType = "REMOVED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ADDED" | "REMOVED" | "UPDATED" | Unrecognized<string>
```