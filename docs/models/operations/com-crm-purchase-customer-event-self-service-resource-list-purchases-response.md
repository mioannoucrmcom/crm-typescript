# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesResponse

OK

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesResponse } from "crm/models/operations";

let value: ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesResponse =
  {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        referenceNumber: "0012345",
        state: "POSTED",
        paymentMediumIdentifier: "424242",
        transactionAmounts: {
          net: 12.11,
          tax: 0.11,
          discount: 1,
          total: 11,
        },
        spendRequest: {
          amount: 2.96,
        },
        date: 1572534147,
        classification: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
        pass: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          code: "2131424123",
        },
        organisation: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "CRMdotCOM Nicosia",
          creatives: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              width: 2159,
              height: 3075,
              format: "jpg",
              url: "https://assets.crm.com/image/offer.jpg",
              publicId: "crm-com/image",
              media: [
                {
                  width: 200,
                  height: 300,
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
        parentOrganisation: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "CRMdotCOM Nicosia",
          creatives: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              width: 2159,
              height: 3075,
              format: "jpg",
              url: "https://assets.crm.com/image/offer.jpg",
              publicId: "crm-com/image",
              media: [
                {
                  width: 200,
                  height: 300,
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
        rewards: {
          award: 121.99,
          spend: 12.22,
          redeem: 12.22,
        },
        adHocReturn: {
          amount: 12.34,
          date: 1589987160,
          referenceNumber: "AHR001",
          returnAmount: 200.99,
          returnSpentAmount: 200.99,
        },
        fees: {
          total: 2.54,
          creditFee: 1.21,
          debitFee: 1.34,
        },
        currencyCode: "EUR",
        totalDefaultCurrency: 0.97,
        exchangeRate: 0.97,
        defaultCurrencyCode: "EUR",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                      | Type                                                                                                                                                                                       | Required                                                                                                                                                                                   | Description                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                                                                   | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesPaging](../../models/operations/com-crm-purchase-customer-event-self-service-resource-list-purchases-paging.md)     | :heavy_minus_sign:                                                                                                                                                                         | N/A                                                                                                                                                                                        |
| `content`                                                                                                                                                                                  | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesContent](../../models/operations/com-crm-purchase-customer-event-self-service-resource-list-purchases-content.md)[] | :heavy_minus_sign:                                                                                                                                                                         | N/A                                                                                                                                                                                        |