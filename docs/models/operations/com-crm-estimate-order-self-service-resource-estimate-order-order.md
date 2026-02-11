# ComCrmEstimateOrderSelfServiceResourceEstimateOrderOrder

## Example Usage

```typescript
import { ComCrmEstimateOrderSelfServiceResourceEstimateOrderOrder } from "crm/models/operations";

let value: ComCrmEstimateOrderSelfServiceResourceEstimateOrderOrder = {
  orderEstimate: {
    orderingAllowed: true,
    fulfilledBy: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Bravo Coffee",
    },
    estimatedDelivery: {
      timeToDelivery: 1,
      uot: "MINUTE",
      deliveredAt: 12345565,
    },
    queue: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
    orderFailureReason: "MINIMUM_COST",
  },
  invoiceEstimate: {
    issuedDate: 123456789,
    dueDate: 123456789,
    currencyCode: "EUR",
    net: 1,
    discount: 1,
    tax: 0.99,
    total: 9.99,
    walletFundsAmount: 5.99,
    discountInclTax: 1,
    accountCredit: 9.99,
    taxCalculationFailed: true,
    taxFailureReason: "INVALID_ADDRESS",
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
    items: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        quantity: 2,
        unitPrice: 10,
        netAmount: 20.5,
        taxAmount: 10,
        subTotal: 200.5,
        period: {
          from: 1651172405,
          to: 1653764405,
        },
        discount: {
          discountAmount: 20.5,
          discountPercentage: 10,
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
        pricing: 11.99,
        inStock: 1,
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
  milestonePlanEstimate: [
    {
      stage: {
        id: "b82648cb-e5f4-53b2-26b3-edca38e3e34f",
        name: "new",
        colour: "FADS876",
      },
      queuePercentage: 10,
      percentage: 5,
    },
  ],
  invalidProducts: [
    {
      product: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
      inStock: 1,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                                                       | Type                                                                                                                                                                                                                        | Required                                                                                                                                                                                                                    | Description                                                                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                        | *string*                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                          | The estimation id                                                                                                                                                                                                           |
| `orderEstimate`                                                                                                                                                                                                             | [operations.OrderOrderEstimate](../../models/operations/order-order-estimate.md)                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                          | An estimation on if the Order can be placed and if yes, then its detailed information that includes fulfillment and invoicing details.                                                                                      |
| `invoiceEstimate`                                                                                                                                                                                                           | [operations.OrderInvoiceEstimate](../../models/operations/order-invoice-estimate.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                          | The outright order’s invoicing information. This invoice estimation includes only physical goods ordered as well as One-Time services. It does not include any invoicing or billing information for ordered termed services |
| `serviceDeliveryEstimate`                                                                                                                                                                                                   | [operations.OrderServiceDeliveryEstimate](../../models/operations/order-service-delivery-estimate.md)[]                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                          | Applicable only when purchasing termed services and/or renting devices.Returns detailed billing information on the ordered termed services as well as details on their subscriptions.                                       |
| `milestonePlanEstimate`                                                                                                                                                                                                     | [operations.OrderMilestonePlanEstimate](../../models/operations/order-milestone-plan-estimate.md)[]                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                          | The Order's milestone plans plus each milestone's amount.                                                                                                                                                                   |
| `invalidProducts`                                                                                                                                                                                                           | [operations.OrderInvalidProduct](../../models/operations/order-invalid-product.md)[]                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                          | List of ordered items which were included in the order but cannot be delivered to the consumer at the time of estimation. Invalid ordered products are excluded from the orders cost estimation.                            |
| `subscriptionEstimationAmount`                                                                                                                                                                                              | *number*                                                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                          | N/A                                                                                                                                                                                                                         |