# ComCrmContactSelfServiceResourceGetCommunitiesState

The community people person's relation state. A person is considered as a valid community person only after they accept the invitation to join the community.

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetCommunitiesState } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetCommunitiesState = "ACCEPTED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PENDING" | "ACCEPTED" | "REJECTED" | Unrecognized<string>
```