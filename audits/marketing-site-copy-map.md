# Marketing site copy map

Internal implementation specification. This file is excluded from the public Mintlify site.

## Narrative spine

**Working category bridge:** A product tour with a brain.

**Product explanation:** A product tour follows a script. Browserbot understands the customer's goal, adapts to the live product, and can guide or act within limits set by the product team.

**System line:** Deterministic goal. Adaptive route. Governed action.

**Recovery line:** Browserbot does not depend on one brittle selector. It can re-resolve controls from the live interface and stop rather than guess when confidence is low.

## Homepage

Keep the current outcome-led hero and page structure. Make surgical changes in the product-experience and control sections.

### Product experience

- **Answer:** Explain what is happening when explanation is enough.
- **Show:** Highlight the right control and guide the customer through the live interface.
- **Do:** Navigate, prepare, or complete an approved action.
- **Route:** Bring in the right person with the request and product context intact.

Supporting copy:

> One request can move between guidance and action. Dubot chooses the safest approved route for the job and verifies where it ends.

### Control

Replace any blanket rule that all writes confirm with:

> Your team decides which effects can run automatically, which require approval, and which remain unavailable.

Add browser-specific context:

> Browserbot works inside the customer's signed-in product session and the permissions enforced there.

Do not add crawler architecture to the homepage.

## `/browserbot`

### Hero

Eyebrow: `BROWSERBOT`

Headline: `A product tour with a brain.`

Body:

> Browserbot understands what the customer is trying to do, finds the right controls in the live product, and can guide or act within limits you set.

Primary CTA: `See Browserbot work`

Secondary CTA: `Talk to us`

### Section sequence

1. **A fixed tour follows your script. Browserbot follows the task.**
   Compare authored sequence, adaptive route, guidance, governed action, and recovery.
2. **A living map of your product.**
   Explain pages, controls, capabilities, journeys, account differences, and configurable recrawls.
3. **When the interface changes, the journey can recover.**
   Explain live re-resolution, safe stopping, journey health, and proposed updates.
4. **From guidance to completion.**
   Show Explain, Navigate, Prepare, Approve, Act, Verify.
5. **Your product sets the limits.**
   Explain automatic, confirm-first, unavailable, permissions, and effect-based governance.
6. **Start with one journey.**
   Keep the current focused-pilot CTA.

### Product tour comparison

| Product tour | Browserbot |
| --- | --- |
| Starts from an authored campaign | Starts from the customer's goal |
| Follows a fixed sequence | Adapts to the live product |
| Explains predefined screens | Can guide, navigate, prepare, or act |
| Must be repaired when targeting breaks | Can recover and flag unhealthy journeys |
| Optimized for onboarding and announcements | Optimized for task completion |

Do not imply that recovery is guaranteed. Consequential steps must stop when the intended target or effect cannot be resolved confidently.

## `/dubot`

Keep the page focused on the system behind the customer experience.

Core sequence:

`Product Map -> Journey -> Live Context -> Policy -> Execution -> Verification`

- **Product Map:** Pages, entities, controls, capabilities, account variants, and last-seen evidence.
- **Journey:** Goal, checkpoints, allowed behavior, success conditions, and fallbacks.
- **Live Context:** Current page, entity, product state, role, and permissions.
- **Policy:** Automatic, confirm-first, or unavailable for the expected effect.
- **Execution:** Browser interaction or a connected action.
- **Verification:** Observed product state plus a reviewable run result.

Browserbot must be described as a delivery surface spanning Show and Do. Do not introduce a fifth public resolution mode.

## `/security`

Add two explicitly separate execution paths.

### Browser execution

- Operates inside the signed-in product session.
- Inherits permissions enforced by the product.
- Uses relevant page and journey context.
- May explain, navigate, prepare, or click according to configured policy.
- Can require approval before a consequential effect.
- Verifies the observed result or reports that it could not continue safely.

### Connected action execution

- Uses a reviewed action contract.
- Keeps authorization and business rules with the customer's product.
- Supports automatic, confirm-first, or unavailable policies.
- Verifies the API or host-product result.
- Produces reviewable history.

Do not publish exact region, retention, rollback, or alerting language until the claims ledger is resolved.

## `/pricing`

- Preserve outcome-based pricing until a separate commercial review.
- Reconcile published audit-log retention with chat and action-log retention before changing the table.
- Remove or avoid any flat-cost-across-accounts claim.

## Release boundary

Use the current marketing design system and composition. Do not attempt to anticipate Rocío's product UI. Existing product illustrations may remain as temporary evidence surfaces, but copy must not label conceptual or future behavior as a completed customer result.
