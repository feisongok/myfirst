# Monica — Tools

Agent-specific tooling for Monica, Marketing Automation Lead. References the shared tool index at `agents/tools/INDEX.md`. *When* each action needs approval is governed by `autonomy.md`, not here — this file covers *how* to use the tools.

## Identity

- **Display name:** Monica
- **Email alias:** _TBD — set up during Post-Creation Admin Checklist_

## Stack

Monica operates a four-tool marketing stack. None of these are in the shared `agents/tools/INDEX.md` yet — they are agent-specific. As each is configured (credentials, API access, webhook endpoints), promote it to a shared tool file under `agents/tools/<tool>.md` and add a row to the index, per `agents/CONVENTIONS.md` § Adding a New Tool.

| Tool | Purpose | Credential | Status |
|------|---------|-----------|--------|
| respond.io | Omnichannel messaging (WhatsApp etc.) — nurture, conversion, retention flows | TBD | Not yet configured |
| HubSpot | CRM + marketing automation — contacts, workflows, reporting | TBD | Not yet configured |
| WordPress | Site, landing pages, lead-capture forms | TBD | Not yet configured |
| Classcard | Class scheduling, attendance, student/booking data — source of lifecycle events | TBD | Not yet configured |

## Integration notes

- **Classcard → respond.io webhook** is the first deliverable. Document the event types, payload shape, field mappings, and the respond.io endpoint here once built, so it's maintainable.
- Keep credentials and endpoint secrets out of this file — reference where they live, don't inline them.
- Test every integration with real payloads before activating (per autonomy L4 → L3 progression).

## Setup checklist (pending)

- [ ] respond.io API / workspace access + webhook endpoint
- [ ] HubSpot account access + private app token
- [ ] WordPress admin / API access
- [ ] Classcard account access + webhook/export capability
- [ ] Email alias for Monica (send-as identity)
