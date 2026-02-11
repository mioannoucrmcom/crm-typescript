# ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsResponse

OK

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsResponse } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "8047448052702285",
        state: "ACTIVE",
        activeServices: 1,
        numberOfDevices: 1,
        firstActivationDate: 1620981309,
        billingInfo: {
          billUpDate: 1620981311,
          nextBillingDate: 1620981311,
          nextPaymentDate: 1620981311,
          oneTimeServices: true,
        },
        terms: {
          billingPeriod: {
            duration: 1,
            uot: "MONTH",
          },
          billingDay: {
            dayOfWeek: "MONDAY",
            dayOfMonth: 5,
            monthOfYear: "JANUARY",
          },
          billingModel: "PRE_BILL",
          paymentMethod: {
            type: "CARD",
            identity: {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              identifier: "Visa *****1234 03/25",
            },
          },
        },
        futureServices: 1,
        startDate: 1620981309,
        inactiveServices: 1,
        draftServices: 1,
        trialServices: 1,
        usageBlocked: true,
        account: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Universal Name",
          number: "23114132",
          currencyCode: "EUR",
        },
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                      | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsPaging](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-paging.md)     | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |
| `content`                                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsContent](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-content.md)[] | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |