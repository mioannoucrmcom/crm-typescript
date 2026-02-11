# ComCrmContactSelfServiceResourceVerifyContactExistsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceVerifyContactExistsResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceVerifyContactExistsResponse = {
  contactExists: true,
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   | Example                                                                                       |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `contactExists`                                                                               | *boolean*                                                                                     | :heavy_minus_sign:                                                                            | Indicates whether a contact using the email or phone provided already exists for the business | true                                                                                          |