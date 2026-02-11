# ListContactAddressesSSResponse

OK

## Example Usage

```typescript
import { ListContactAddressesSSResponse } from "crmcom/models/operations";

let value: ListContactAddressesSSResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      type: "HOME",
      name: "Mum's house",
      isPrimary: true,
      addressLine1: "21 Elia Papakyriakou",
      addressLine2: "7 Stars Tower",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2415",
      countryCode: "CYP",
      lat: 35.157115,
      lon: 33.313719,
      googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
    },
  ],
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                   | [operations.ListContactAddressesSSPaging](../../models/operations/list-contact-addresses-ss-paging.md)     | :heavy_minus_sign:                                                                                         | N/A                                                                                                        |
| `content`                                                                                                  | [operations.ListContactAddressesSSContent](../../models/operations/list-contact-addresses-ss-content.md)[] | :heavy_minus_sign:                                                                                         | N/A                                                                                                        |