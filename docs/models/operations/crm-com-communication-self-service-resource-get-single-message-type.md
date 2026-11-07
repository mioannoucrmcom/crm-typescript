# CrmComCommunicationSelfServiceResourceGetSingleMessageType

The message type that a provisioning provider will send (applicable and required only if the selected integrator is a provisioning provider)
 * `MAIL` - Email Communication (send by provisioning provider)
 * `OSD` - On Screen Display Communication (send by provisioning provider)


## Example Usage

```typescript
import { CrmComCommunicationSelfServiceResourceGetSingleMessageType } from "crm/models/operations";

let value: CrmComCommunicationSelfServiceResourceGetSingleMessageType = "MAIL";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"MAIL" | "OSD" | Unrecognized<string>
```