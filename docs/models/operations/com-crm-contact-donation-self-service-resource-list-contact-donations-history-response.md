# ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryResponse

OK

## Example Usage

```typescript
import { ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryResponse } from "crmcom/models/operations";

let value:
  ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryResponse =
    {
      paging: {
        page: 2,
        size: 20,
        total: 5124,
        hasMore: true,
      },
      content: [
        {
          amount: 40,
          currencyCode: "EUR",
          donationOffer: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
          organisation: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
          date: 1589796854,
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                       | Type                                                                                                                                                                                                        | Required                                                                                                                                                                                                    | Description                                                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                                    | [operations.ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryPaging](../../models/operations/com-crm-contact-donation-self-service-resource-list-contact-donations-history-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                          | N/A                                                                                                                                                                                                         |
| `content`                                                                                                                                                                                                   | [operations.ComCrmContactDonationSelfServiceResourceListContactDonationsHistoryContent](../../models/operations/com-crm-contact-donation-self-service-resource-list-contact-donations-history-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                          | N/A                                                                                                                                                                                                         |