# ComCrmApplicationSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceListResponse } from "crm/models/operations";

let value: ComCrmApplicationSelfServiceResourceListResponse = {
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      type: "PAYMENT_GATEWAYS",
      connector: "JCC",
      mediaUrl: "crm.com/provider.png",
      organisation: {
        id: "d40a5bdf-2077-8c22-ea8e-8a0709f15fe0",
        type: "BUSINESS",
      },
      paymentGateways: {
        isRewards: true,
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                             | Type                                                                                                                                              | Required                                                                                                                                          | Description                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                                         | [operations.ComCrmApplicationSelfServiceResourceListContent](../../models/operations/com-crm-application-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                | N/A                                                                                                                                               |