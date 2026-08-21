# Browserbot claims ledger

Internal review artifact. This file is excluded from the public Mintlify site.

Status vocabulary:

- **Available now:** Supported in the current product.
- **Available for evaluation:** Can be tested through a scoped customer journey, but is not a general-availability commitment.
- **Committed capability:** Approved product promise that may extend beyond the current implementation.
- **Unresolved:** Must not be stated precisely until the named owner confirms it.

| Claim | Status | Public destination | Approved framing | Verification required |
| --- | --- | --- | --- | --- |
| Browserbot can guide, navigate, fill, and click | Available for evaluation | Homepage, Browserbot, docs | Browserbot can guide or act through the live product within limits set by the product team. | Verify the exact supported step types in the evaluation environment. |
| A Browserbot journey can contain both Show and Do behavior | Available for evaluation | Browserbot, Dubot, docs | Show and Do describe behavior inside a journey. Browserbot is the adaptive surface that delivers it. | Confirm which current journeys demonstrate both behaviors end to end. |
| Guidance is created manually or promoted from exploration | Available now | Docs | Teams can author guidance or promote an explored journey into a reviewed guide. | None. |
| Runtime recovery uses current page evidence | Available for evaluation | Browserbot, docs | Browserbot resolves the next step against the live interface and can recover when a saved target no longer matches. | Confirm the production confidence and safe-stop thresholds before publishing stronger reliability language. |
| Dubot will crawl logged-in products to build a product map | Committed capability | Browserbot, Dubot, docs | Dubot builds a living map of pages, controls, capabilities, and journeys. | Do not attach a delivery date until engineering confirms one. |
| Recrawls identify product changes and propose journey updates | Committed capability | Browserbot, docs | Configurable recrawls identify unhealthy journeys and propose updates for review. | Confirm initial recrawl frequency options and review workflow. |
| Account differences are handled without copying every journey | Committed capability | Browserbot, docs | Shared product meaning is combined with account-specific roles, labels, fields, features, and routes. | Confirm the persisted account-overlay model before documenting configuration fields. |
| Actions support automatic, confirm-first, and unavailable policies | Available now | Homepage, Browserbot, docs, security | The product team decides which effects run automatically, require approval, or remain unavailable. | Confirm whether any categories are forced to confirm regardless of configuration. |
| Approval is enforced by the SDK | Available now | Docs, security | Confirm-first actions require a person to approve the resolved action before it runs. | Confirm identity and audit fields captured with approval. |
| Browser execution uses the customer's authenticated product session | Available for evaluation | Docs, security | Browserbot operates inside the signed-in product session and inherits the permissions enforced by the product. | Confirm behavior across supported browser and SDK environments. |
| Relevant chats and page interaction data can be processed by Dubot and the selected model provider | Available now | Docs, security | Relevant journey context may be processed by Dubot and the configured model provider. | Document the exact minimization, redaction, and customer-control options. |
| Admin runs on Node and AWS ECS, SDK traffic uses Cloudflare Workers, and analytics is queued to ClickHouse | Available now | Architecture docs | Describe the service roles without publishing an unverified region. | Confirm current deployment and backup architecture before publication. |
| Dubot supports multiple model providers and does not train a foundation model | Available now | Docs | Dubot works with multiple model providers; customers can evaluate the provider that fits their requirements. | Confirm the supported-provider list and bring-your-own-model boundary. |
| Configuration is retained until account deletion | Unresolved | Security, privacy | Do not publish a duration yet. | Confirm deletion, backup, and legal-hold behavior. |
| Chats and action logs are retained for three or six months | Unresolved | Security, pricing, privacy | Do not publish until the data-category and plan mapping is explicit. | Reconcile with the pricing page's audit-log retention table. |
| Failed runs appear in the dashboard and scheduled digest | Unresolved | Docs | Describe only after verifying the live product. | Confirm shipped status, timing, recipients, and configuration. |
| Real-time failure webhooks are available | Unresolved | Docs | Do not promise. | Engineering confirmation and delivery status. |
| Dubot provides generic rollback | Unresolved | Security, docs | Do not promise generic rollback. Reversal requires a product-specific compensating action or supported UI flow. | Confirm whether any current action types expose undo. |
| Cost to serve is flat across accounts | Unresolved | Pricing and sales | Do not use this claim. | Model crawl scope, page variance, journey count, run volume, recovery frequency, model selection, and assistance. |
| Third-party browser agents must obey Dubot policy | Unresolved | MCP, security | Policy is enforceable when an agent invokes a Dubot-governed capability. Dubot cannot guarantee compliance when an agent bypasses Dubot and independently drives the UI. | Define the external-agent enforcement and revocation model. |
| Product actions are available to external agents over MCP | In development | MCP docs | Keep workspace administration MCP separate from customer-product action execution. | Prototype scoped customer-product authorization and verified receipts before claiming availability. |

## Publication rule

Marketing may lead with a committed outcome, including crawl-led product mapping, without exposing implementation details. Technical documentation must continue to label current, evaluable, committed, and unresolved behavior. Security and privacy statements require current engineering evidence and, where appropriate, legal review.
