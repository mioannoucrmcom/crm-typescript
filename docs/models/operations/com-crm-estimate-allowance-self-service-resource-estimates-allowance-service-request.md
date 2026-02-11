# ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceRequest

The identifier of the service through which usage is consumed. If not specified, then the response will include all termed and one-time services that allow the specified contact to consume usage. In the latter case, one-time services which are expired or fully consumed are not returned. For termed services, only non-cancelled ones are returned

## Example Usage

```typescript
import { ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceRequest } from "crmcom/models/operations";

let value:
  ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceRequest = {
    id: "<id>",
    classification: "ONE_TIME_SERVICE",
  };
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           | Example                                                                               |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `id`                                                                                  | *string*                                                                              | :heavy_check_mark:                                                                    | The unique identifier of the service                                                  |                                                                                       |
| `classification`                                                                      | [operations.ClassificationRequest](../../models/operations/classification-request.md) | :heavy_check_mark:                                                                    | The contact (identifier) that will be authorised                                      | ba48e7d3-d00a-0d28-4f9f-02b1a5b226bc                                                  |