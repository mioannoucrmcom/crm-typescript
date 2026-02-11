# ComCrmContactSelfServiceResourceActionRequestBody

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceActionRequestBody } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceActionRequestBody = {
  action: "REJECT",
};
```

## Fields

| Field                                                                                                                                                                                        | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `action`                                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceActionAction](../../models/operations/com-crm-contact-self-service-resource-action-action.md)                                                    | :heavy_check_mark:                                                                                                                                                                           | The action to be performed on the contact relatioship status<br/> * `ACCEPT` - Accept the invitation to be part of a community<br/> * `REJECT` - Accept the invitation to be part of a community<br/> |