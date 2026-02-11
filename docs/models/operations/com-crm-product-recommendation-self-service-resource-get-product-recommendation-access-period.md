# ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationAccessPeriod

The period of time that contacts will have access to the service. Applicable only for one-time services. Either the billing period or the access period should be specified for one-time services.

## Example Usage

```typescript
import {
  ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationAccessPeriod,
} from "crm/models/operations";

let value:
  ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationAccessPeriod =
    {
      startDate: 1612953199,
      endDate: 1612953199,
    };
```

## Fields

| Field                                         | Type                                          | Required                                      | Description                                   | Example                                       |
| --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| `startDate`                                   | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will start | 1612953199                                    |
| `endDate`                                     | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will end   | 1612953199                                    |