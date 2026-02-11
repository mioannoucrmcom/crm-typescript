# ComCrmEstimateSelfServiceResourceEstimateInvoicingResponse

OK

## Example Usage

```typescript
import { ComCrmEstimateSelfServiceResourceEstimateInvoicingResponse } from "crmcom/models/operations";

let value: ComCrmEstimateSelfServiceResourceEstimateInvoicingResponse = {
  issuedDate: 1642457163,
  dueDate: 1642457163,
  currencyCode: "EUR",
  totalNetAmount: 45.5,
  walletFundsAmount: 5.99,
  isCredit: true,
  lines: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      quantity: 2,
      unitPrice: 10,
      net: 20.5,
      tax: 10,
      subTotal: 200.5,
      period: {
        from: 1651172405,
        to: 1653764405,
      },
      discount: {
        amount: 20.5,
        percentage: 10,
        amountInclTax: 15.5,
      },
      product: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        sku: "CBL-54455",
        name: "Cable",
        classification: "TRACEABLE_PHYSICAL_GOOD",
        isStockable: false,
      },
      bundleProduct: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        sku: "CBL-54455",
        name: "Cable",
        classification: "TRACEABLE_PHYSICAL_GOOD",
        isStockable: false,
      },
      appliedTaxes: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          taxRate: {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            name: "VAT",
            taxCode: "VAT",
          },
          taxAmount: 1.5,
          taxExemptReason: "PRODUCT",
        },
      ],
      pricing: 9.99,
    },
  ],
  taxesBreakdown: [
    {
      taxRate: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "VAT",
        taxCode: "VAT",
      },
      taxAmount: 1.5,
      taxExemptReason: "PRODUCT",
    },
  ],
  discounts: [
    {
      amount: 2,
      type: "AD_HOC",
      promotion: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                     | Type                                                                                                                                                                                      | Required                                                                                                                                                                                  | Description                                                                                                                                                                               | Example                                                                                                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `issuedDate`                                                                                                                                                                              | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | The estimated invoice issued date                                                                                                                                                         | 1642457163                                                                                                                                                                                |
| `dueDate`                                                                                                                                                                                 | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | The estimated invoice due date                                                                                                                                                            | 1642457163                                                                                                                                                                                |
| `currencyCode`                                                                                                                                                                            | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingCurrencyCode](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-currency-code.md)           | :heavy_minus_sign:                                                                                                                                                                        | The estimated invoice currency. 3-letter ISO 4217 currency code.                                                                                                                          | EUR                                                                                                                                                                                       |
| `totalNetAmount`                                                                                                                                                                          | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       | 45.5                                                                                                                                                                                      |
| `totalDiscountAmount`                                                                                                                                                                     | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `totalTaxAmount`                                                                                                                                                                          | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `totalAmount`                                                                                                                                                                             | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `walletFundsAmount`                                                                                                                                                                       | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       | 5.99                                                                                                                                                                                      |
| `isCredit`                                                                                                                                                                                | *boolean*                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       | true                                                                                                                                                                                      |
| `totalDiscountInclTax`                                                                                                                                                                    | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `amountDue`                                                                                                                                                                               | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `amountToCollect`                                                                                                                                                                         | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `totalPrice`                                                                                                                                                                              | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | Sum of all product prices as these are defined in the product catalog                                                                                                                     |                                                                                                                                                                                           |
| `accountFunds`                                                                                                                                                                            | *number*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `lines`                                                                                                                                                                                   | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingLine](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-line.md)[]                          | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `taxesBreakdown`                                                                                                                                                                          | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingTaxesBreakdown](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-taxes-breakdown.md)[]     | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |
| `discounts`                                                                                                                                                                               | [operations.ComCrmEstimateSelfServiceResourceEstimateInvoicingDiscountResponse](../../models/operations/com-crm-estimate-self-service-resource-estimate-invoicing-discount-response.md)[] | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |                                                                                                                                                                                           |