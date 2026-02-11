# ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionResponse

Created

## Example Usage

```typescript
import { ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionResponse } from "crm/models/operations";

let value:
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionResponse = {
    serviceDeliveryEstimate: [
      {
        actionAllowed: true,
        allowedExecutionOn: 12345678,
        nextBillingAt: 1235678,
        nextPaymentDate: 12345678,
        subscription: {
          state: "ACTIVE",
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
          },
        },
        billingEstimate: {
          billedPeriod: {
            fromDate: 12345678,
            toDate: 12345678,
          },
          totals: {
            totalAmount: 9.99,
            taxAmount: 1.99,
            netAmount: 1.99,
            discountAmount: 1.99,
          },
          invoicing: [
            {
              issuedDate: 123456789,
              dueDate: 123456789,
              currencyCode: "EUR",
              totalNetAmount: 1,
              totalDiscountAmount: 1,
              totalTaxAmount: 0.99,
              totalAmount: 9.99,
              walletFundsAmount: 5.99,
              totalDiscountInclTax: 1,
              taxCalculationFailed: true,
              taxFailureReason: "INVALID_ADDRESS",
              taxesBreakdown: [
                {
                  taxRate: {
                    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                    taxCode: "VAT",
                    percentage: 1,
                  },
                  taxAmount: 0.99,
                },
              ],
              lineItems: [
                {
                  quantity: 1,
                  unitPrice: 9.99,
                  netAmount: 9.99,
                  taxAmount: 0.99,
                  subTotal: 9.99,
                  pricing: 11.99,
                  discount: {
                    discountAmount: 0.96,
                    discountPercentage: 1.5,
                    discountInclTax: 0.98,
                  },
                  product: {
                    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                    name: "Decoder",
                    sku: "DEC1234",
                    classification: "TRACEABLE_PHYSICAL_GOOD",
                  },
                  bundleProduct: {
                    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                    name: "Decoder",
                    sku: "DEC1234",
                    classification: "TRACEABLE_PHYSICAL_GOOD",
                  },
                  appliedTaxes: [
                    {
                      taxRate: {
                        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                        taxCode: "VAT",
                        percentage: 1,
                      },
                      taxAmount: 0.99,
                      taxExemptReason: "CONTACT",
                    },
                  ],
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
            },
          ],
          billingDate: 12345678,
        },
        componentsChange: {
          service: {
            id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
            name: "Universal Name",
            sku: "S0001",
          },
          componentsAdded: [
            {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          ],
          componentsRemoved: [
            {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          ],
        },
        servicesToAdd: [
          {
            state: "EFFECTIVE",
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
            trialPeriod: {
              startsOn: 12345678,
              endsOn: 12345678,
            },
            quantity: 5,
            components: [
              {
                id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                quantity: 5,
              },
            ],
          },
        ],
        servicesToRemove: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            state: "EFFECTIVE",
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          },
        ],
        servicesToChange: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            state: "EFFECTIVE",
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
            changeToProduct: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          },
        ],
        servicesToUpdate: [
          {
            state: "EFFECTIVE",
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
            trialPeriod: {
              startsOn: 12345678,
              endsOn: 12345678,
            },
            quantity: 5,
            components: [
              {
                id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                quantity: 5,
              },
            ],
          },
        ],
        devicesAdded: [
          {
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                                                   | Type                                                                                                                                                                                                                                    | Required                                                                                                                                                                                                                                | Description                                                                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `serviceDeliveryEstimate`                                                                                                                                                                                                               | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionServiceDeliveryEstimate](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-service-delivery-estimate.md)[] | :heavy_minus_sign:                                                                                                                                                                                                                      | N/A                                                                                                                                                                                                                                     |