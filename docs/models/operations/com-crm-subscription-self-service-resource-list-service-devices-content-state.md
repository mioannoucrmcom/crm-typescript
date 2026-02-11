# ComCrmSubscriptionSelfServiceResourceListServiceDevicesContentState

Defines whether the service is already enabled on the device or not. If disabled, then the service can be enabled on the related device

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListServiceDevicesContentState } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceListServiceDevicesContentState =
  "ENABLED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DISABLED" | "ENABLED" | Unrecognized<string>
```