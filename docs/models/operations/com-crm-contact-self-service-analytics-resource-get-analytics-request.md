# ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsRequest = {
  id: "02b0fb6c-cdb1-4a7d-a938-53ea2c01e253",
  frequency: "<value>",
  metrics: "<value>",
};
```

## Fields

| Field                                                                                                                          | Type                                                                                                                           | Required                                                                                                                       | Description                                                                                                                    | Example                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                           | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | The contact identifier that analytics will be retrieved                                                                        | 02b0fb6c-cdb1-4a7d-a938-53ea2c01e253                                                                                           |
| `frequency`                                                                                                                    | *string*                                                                                                                       | :heavy_check_mark:                                                                                                             | Frequency denotes which metric will be applied for example get the metrics of this month                                       |                                                                                                                                |
| `metrics`                                                                                                                      | *any*                                                                                                                          | :heavy_check_mark:                                                                                                             | Which metrics are required. A list of metrics can be included in the request, comma separated. At least one must be specified. |                                                                                                                                |