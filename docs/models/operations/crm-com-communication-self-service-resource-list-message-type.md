# CrmComCommunicationSelfServiceResourceListMessageType

The message type that a provisioning provider will send (applicable and required only if the selected integrator is a provisioning provider)
 * `MAIL` - Email Communication (send by provisioning provider)
 * `OSD` - On Screen Display Communication (send by provisioning provider)


## Example Usage

```typescript
import { CrmComCommunicationSelfServiceResourceListMessageType } from "crmcom/models/operations";

let value: CrmComCommunicationSelfServiceResourceListMessageType = "OSD";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"MAIL" | "OSD" | Unrecognized<string>
```