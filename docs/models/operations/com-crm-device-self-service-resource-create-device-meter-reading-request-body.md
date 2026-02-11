# ComCrmDeviceSelfServiceResourceCreateDeviceMeterReadingRequestBody

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceCreateDeviceMeterReadingRequestBody } from "crmcom/models/operations";

let value: ComCrmDeviceSelfServiceResourceCreateDeviceMeterReadingRequestBody =
  {
    reading: 1.09,
    dates: {
      from: 1683547447,
      to: 1683547447,
    },
  };
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               | Example                                                                                   |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `reading`                                                                                 | *number*                                                                                  | :heavy_check_mark:                                                                        | The meter reading that will be added to the device                                        | 1.09                                                                                      |
| `dates`                                                                                   | [operations.Dates](../../models/operations/dates.md)                                      | :heavy_minus_sign:                                                                        | The date on which such reading was performed (if not specified, current date will be set) |                                                                                           |