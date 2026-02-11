# ComCrmServiceRequestSelfServiceResourceListAddress

Details about the address

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceListAddress } from "crmcom/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceListAddress = {
  addressType: "HOME",
  addressName: "My house",
};
```

## Fields

| Field                                 | Type                                  | Required                              | Description                           | Example                               |
| ------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- |
| `id`                                  | *string*                              | :heavy_minus_sign:                    | The contact address unique identifier |                                       |
| `addressType`                         | *string*                              | :heavy_minus_sign:                    | The address type                      | HOME                                  |
| `addressName`                         | *string*                              | :heavy_minus_sign:                    | The address name                      | My house                              |
| `addressLine1`                        | *string*                              | :heavy_minus_sign:                    | The address line 1                    |                                       |
| `addressLine2`                        | *string*                              | :heavy_minus_sign:                    | The address line 2                    |                                       |
| `stateProvinceCounty`                 | *string*                              | :heavy_minus_sign:                    | The address state/province/county     |                                       |
| `townCity`                            | *string*                              | :heavy_minus_sign:                    | The address town/city                 |                                       |
| `postalCode`                          | *string*                              | :heavy_minus_sign:                    | The address postal code               |                                       |
| `countryCode`                         | *string*                              | :heavy_minus_sign:                    | The address country code              |                                       |
| `lat`                                 | *number*                              | :heavy_minus_sign:                    | The address geolocation latitude      |                                       |
| `lon`                                 | *number*                              | :heavy_minus_sign:                    | The address geolocation longtitude    |                                       |
| `googlePlaceId`                       | *string*                              | :heavy_minus_sign:                    | The address unique Google identifier  |                                       |