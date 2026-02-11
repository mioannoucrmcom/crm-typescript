# ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsResponse

OK

## Example Usage

```typescript
import { ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsResponse } from "crmcom/models/operations";

let value:
  ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        usageAmount: 1.99,
        usageTimestamp: 12345678,
        createdDate: 12345678,
        chargedAmount: 1.99,
        currencyCode: "EUR",
        billedAmount: 1.99,
        state: "POSTED",
        usageProduct: {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "Universal Name",
          sku: "S0001",
        },
        service: {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "Universal Name",
          sku: "S0001",
        },
        organisation: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
        measurementUnit: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Gigabytes",
          displayName: "GB",
        },
        invoice: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          number: "EHD001",
          referenceNumber: "425235434243234",
        },
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                  | Type                                                                                                                                                                                                   | Required                                                                                                                                                                                               | Description                                                                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                                                                               | [operations.ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsPaging](../../models/operations/com-crm-usage-detail-record-self-service-resource-list-usage-detail-records-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                     | N/A                                                                                                                                                                                                    |
| `content`                                                                                                                                                                                              | [operations.ComCrmUsageDetailRecordSelfServiceResourceListUsageDetailRecordsContent](../../models/operations/com-crm-usage-detail-record-self-service-resource-list-usage-detail-records-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                     | N/A                                                                                                                                                                                                    |