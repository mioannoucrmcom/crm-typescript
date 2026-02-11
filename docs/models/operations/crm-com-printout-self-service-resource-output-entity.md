# CrmComPrintoutSelfServiceResourceOutputEntity

Defines the entity based on which the printout will be created

## Example Usage

```typescript
import { CrmComPrintoutSelfServiceResourceOutputEntity } from "crmcom/models/operations";

let value: CrmComPrintoutSelfServiceResourceOutputEntity = {
  type: "INVOICE",
  id: "007c08166f95-8c54d563-b991-4b76-8a83",
};
```

## Fields

| Field                                                                                                                                   | Type                                                                                                                                    | Required                                                                                                                                | Description                                                                                                                             | Example                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                  | [operations.CrmComPrintoutSelfServiceResourceOutputType](../../models/operations/crm-com-printout-self-service-resource-output-type.md) | :heavy_check_mark:                                                                                                                      | The entity type                                                                                                                         | INVOICE                                                                                                                                 |
| `id`                                                                                                                                    | *string*                                                                                                                                | :heavy_minus_sign:                                                                                                                      | The entity identifier (e.g. invoice id)                                                                                                 | 007c08166f95-8c54d563-b991-4b76-8a83                                                                                                    |