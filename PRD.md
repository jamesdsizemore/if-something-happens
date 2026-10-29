# If Something Happens

## Product Requirements Document

Version 1.0 · October 29, 2026  
Scope: first production release of a mobile application for preparing a household and coordinating a loved one's response to a serious emergency, incapacity, or death.

This document defines the product to build, its behavior, release boundaries, and acceptance criteria. Requirements are product decisions for this specification; research evidence is cited separately. It supersedes the discovery record's unresolved scope discussion as the working implementation baseline. No earlier generated screen is an approved design.

## 1. Product definition

**If Something Happens gives the people someone trusts a usable plan for handling that person's affairs when they cannot do so themselves or have died.**

The product connects personal records to concrete work: what exists, which situation makes it relevant, who needs to act, whom to contact, what to gather, how to proceed, and how to know whether the work is complete. It supports advance preparation and a loved one starting after an event without a prepared plan.

A policy entry is connected to its insurer, employer when applicable, beneficiary information, evidence of actual coverage, documents, and claim process. A digital-account entry is connected to the owner's wishes, platform permissions, access prerequisites, preservation needs, dependent services, and the permitted route to the desired outcome. A task remains connected to these records throughout follow-through.

### Product promise

A loved one can find the important information, understand the next useful action, prepare what is needed, coordinate help, and track the result without reconstructing the person's affairs across unrelated documents and conversations.

### Problem being solved

Information is fragmented across employer portals, insurance documents, bank statements, devices, email, personal conversations, and institutional processes. The person responding may be grieving, under immediate pressure, unfamiliar with the institutions, or unable to obtain information directly from the owner. Institutional authority and documentation requirements differ. Some actions remove access or destroy options needed by later work.

Success means fewer lost handoffs, missing prerequisites, repeated explanations, overlooked benefits, and preventable interruptions. The product does not determine an insurer's liability, adjudicate inheritance, or grant rights over an external account.

## 2. Users and ownership model

| User | Primary responsibility in the product | Essential outcome |
| --- | --- | --- |
| Plan owner | Organize their own information, record wishes, select recipients, and maintain current records. | Someone else can use the plan independently when needed. |
| Loved one responding to an event | Start a response workspace, find relevant information, and perform or coordinate work. | Know what to do next and what remains unresolved. |
| Family helper | Complete assigned work and contribute permitted information. | Help without gaining unnecessary access to the person's entire affairs. |
| Estate or other legal representative | Record their role and evidence, coordinate applicable institutional processes. | Use the relevant information while keeping institutional requirements explicit. |
| Beneficiary | Follow a benefit-specific claim process for their own entitlement. | Submit the appropriate claim and track its outcome separately from other beneficiaries. |

Product permissions and external legal roles are separate. An executor can also be a beneficiary and a helper; the product records each role without treating one as proof of another.

Each adult owns their own plan. A household links plans for navigation but does not merge ownership, consent, beneficiaries, or permissions. The product must remain usable when both partners are affected by the same event.

## 3. Release decisions and boundaries

### Included in the first production release

- iOS and Android applications using the same core product behavior and synchronized records.
- Preparation of a personal plan, permissioned sharing, and a verified recipient handoff.
- Separate response paths for serious illness/injury or incapacity and for death.
- A response workspace that can be started without the affected person having used the product.
- Private insurance, employer benefits, financial-account references, important documents, contacts, household continuity, personal wishes, and digital affairs.
- An actionable task system with prerequisites, assignments, evidence, provider handoffs, deadline provenance, and follow-up history.
- Claim and request preparation: structured checklists, document selection, reusable factual information, request drafts, and exportable packages.
- Links and handoffs to official submission channels; users record submissions, responses, payments, and other outcomes.
- Offline access to a deliberately saved emergency summary and an export that can be used without this service.

### External action boundary

The release is interactive: people create and manage real cases, gather evidence, prepare packages, coordinate work, and record outcomes. It does not claim to execute every institution's transactions.

Direct third-party submission, account control, or status retrieval is exposed only for a specific integration that meets the integration contract in section 12. **The initial release has no dependency on a carrier, bank, government, or social platform approving such access.** Its complete supported route is preparation plus a documented handoff to the recognized institution channel.

Browser automation, a stored password, or a generic financial-data connection is not accepted as proof that the product can submit a survivor claim, transfer an estate asset, or control a deceased person's profile. No release feature impersonates the affected person.

### Explicitly excluded from this release

- Executing bank transfers, receiving or holding benefit proceeds, or distributing estate assets.
- Automatic eligibility decisions, promised payouts, or aggregate “money you will receive” estimates.
- Issuing legal documents, appointing representatives, establishing guardianship, or replacing an institution's authority review.
- Automatic death detection, automatic disclosure of private records after inactivity, or new access granted solely because someone reports a death.
- Autonomous submission of claims or irreversible closure, deletion, or transfer of external accounts.
- A password-manager replacement, storage of cryptocurrency seed phrases, or automatic credential retrieval.
- Medical triage, treatment recommendations, emergency dispatch, or an on-demand human case-management service.

### Geography and content coverage

The first release serves U.S. households in English. Federal and institution-specific procedures are supported nationally. State-specific instructions are displayed only for a jurisdiction with reviewed, maintained content for the specific action. Elsewhere, the task identifies the relevant local court, authority, institution, or professional to contact and the information to request; it does not invent a national rule.

International records may be stored. Their response tasks use institution contact and document collection rather than unsupported jurisdiction-specific instructions.

### Commercial access

Initial release is a free, controlled launch without billing. Responders do not encounter an upgrade gate for reading shared information, carrying out supported tasks, or exporting their permitted records. A later commercial model must preserve these response capabilities for existing shared plans and active cases.

## 4. Product principles

1. **Useful before complete.** A name and one contact can start a plan; missing information becomes work to resolve.
2. **Show the next action and why it matters.** A large inventory is not a response plan.
3. **Separate facts from possibilities.** An uploaded brochure, an enrolled benefit, a beneficiary designation, and an approved claim have different meanings.
4. **Respect roles and wishes.** Sharing information does not make someone a beneficiary or legal representative.
5. **Preserve options.** Retrieval, continuity, and access dependencies precede irreversible account actions where applicable.
6. **Carry context forward.** The person should not repeatedly re-enter the same factual details to prepare related work.
7. **Keep the user in control.** Exports and any supported external actions identify exactly what is being shared and with whom.
8. **Use calm, practical language.** No completion celebrations, streaks, pressure to finish a plan, or assumptions about how someone feels.

## 5. Primary journeys

### J1 — Prepare and hand off a plan

1. Owner creates an account and a plan in their own name.
2. Adds an initial trusted recipient and chooses which existing records to share. New records default to private.
3. Adds employer, insurer, financial, document, digital-account, and wishes records progressively; unknown details are allowed.
4. Recipient accepts through their own verified account. Owner confirms the recipient identity and the selected grant.
5. Recipient opens a handoff rehearsal, locates a shared contact and document, and confirms they know where to start.
6. Owner receives a precise readiness summary: what is shared, which recipients completed rehearsal, what remains private, and which records need review.

**Completion:** at least one confirmed recipient has independently opened the shared plan and completed a rehearsal. Merely entering an email does not establish readiness.

### J2 — Medical emergency or incapacity with an existing plan

1. Recipient opens the plan under their own account and starts a living-person response case.
2. Records the situation, whether immediate professional help is already being handled, and the information currently known. The product provides a visible local emergency-call route when immediate help is needed; it does not diagnose.
3. Sees the permitted emergency contacts, relevant wishes/directives, insurance information, dependent-care arrangements, and document locations.
4. Activates applicable employer leave/disability, medical coverage, household-continuity, and representative-access tasks.
5. Assigns work to permitted helpers, prepares relevant information, follows official channels, and records outcomes.
6. Records recovery, ongoing incapacity, or a subsequent death. Historical work remains intact; new event-specific tasks are added without duplicating completed notifications blindly.

**Completion:** relevant work is resolved or deliberately deferred with a recorded reason and follow-up; an emergency ending does not imply every financial or insurance task is finished.

### J3 — Death with an existing plan

1. Recipient starts a death-response case and records the date and known location. The event is identified as reported by that user, not independently certified by the app.
2. Establishes which immediate arrangements are already handled and locates wishes, funeral arrangements, relevant documents, and contacts.
3. Identifies involved beneficiaries, helpers, and estate representatives as separate roles.
4. Works through applicable employer/insurance claims, survivor income and coverage, household continuity, banking/estate processes, and digital affairs.
5. Prepares institution-specific document packages, follows the institution's submission route, and tracks acknowledgment, missing information, decisions, and outcomes.
6. Preserves an exportable case record, including what remains pending. Archiving requires resolution or explicit disposition of active work.

### J4 — Start after an event without a prepared plan

1. Loved one creates a workspace for the affected person, records their relationship and claimed role, and chooses the event type.
2. Supplies whatever is known; neither an account inventory nor a policy number is required to begin.
3. Receives discovery tasks: contact the employer, locate records, identify institutions and representatives, and use applicable official locator services.
4. Adds records, contacts, and evidence as found. Potential benefits remain unconfirmed until supported by specific evidence.
5. Invites helpers with limited case permissions and follows the same supported workflows.

**Boundary:** this route never reveals a private plan merely because the person's name or email matches an existing owner. Separate workspaces are not merged automatically.

### J5 — Settle digital affairs

1. Selects the account or digital asset and reviews the recorded wishes, provider procedure, available role, and connected services.
2. Establishes the permitted objective: retrieve data, maintain permitted administration, transfer an eligible asset, memorialize, close, or retain.
3. Resolves required keys, identity/authority documents, preservation steps, and service dependencies.
4. Prepares the relevant request and follows the official channel under the requester's own identity.
5. Records the provider response and confirms each component's outcome separately. Domain access does not complete hosting, email, or business administration tasks.

## 6. Functional requirements — preparation and records

Priority **P0** is required for release. **P1** is the next increment and must not be represented as launch functionality.

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| PLAN-01 | P0 | Create a plan with minimal information. | Name is sufficient to start. Unknown provider, policy, beneficiary, account, or document details do not prevent saving. |
| PLAN-02 | P0 | Maintain structured records and their provenance. | Each record shows who supplied it, source/reference when available, last review date, sharing scope, and confidence/verification category. |
| PLAN-03 | P0 | Connect records. | A benefit can link employer, carrier, contacts, beneficiary information, documents, and tasks without duplicating the source record. |
| PLAN-04 | P0 | Preserve changes. | Replacing coverage or a document retains the prior version and identifies affected active cases. A historical claim keeps its original evidence references. |
| PLAN-05 | P0 | Maintain named primary and fallback contacts. | Owner can distinguish personal helper, employer administrator, provider contact, attorney, and other roles; contact failure can be recorded with an alternate route. |
| PLAN-06 | P0 | Explain readiness specifically. | Show missing contacts, unknown coverage, stale records, unaccepted grants, and uncompleted rehearsals. Do not collapse these into an unsupported percentage of preparedness. |
| PLAN-07 | P0 | Support maintenance. | Owner receives an annual review prompt and can request review after employer, household, beneficiary, or provider changes. Prompts identify records to review. |
| PLAN-08 | P0 | Capture personal wishes and legal-document locations. | Record funeral/disposition preferences, notification wishes, dependent/pet-care instructions, personal messages, and relevant document locations. Informal wishes and uploaded legal documents remain distinct. |
| PLAN-09 | P0 | Export a permitted plan. | User selects records and attachments; export includes a human-readable index, source dates, current permissions context, and clear missing-data labels. |
| PLAN-10 | P1 | Assist extraction from supported documents. | Extracted values are proposed with page references and require review before becoming record facts. Manual entry remains complete and available. |

### Required record families

| Record | Required capability and conditional fields |
| --- | --- |
| Person | Identity/contact information, relationships, declared roles, and jurisdiction relevant to a case. Sensitive details are optional until a task requires them. |
| Employer | Employer/union, employment status, HR/benefits administrator, official contact routes, known plans, source documents, final-pay/retirement inquiry references. |
| Benefit/policy | Type, insurer/administrator, private or employer source, member/group/policy references, covered person, elected coverage, effective/end dates when known, beneficiary evidence, exclusions/conditions references, claim route, and verification status. |
| Financial account | Institution, account category, masked reference, ownership/beneficiary information as supplied, estate contact route, related bills, document references, and institution-verification status. No transaction access is inferred. |
| Document | Type, owner/uploader, subject, issue/review date, version, storage/location, visibility, source, and cases/tasks that reference it. |
| Digital asset | Provider, account/asset type, URL/handle, personal/business distinction, intended outcome, platform designations, separate administrators, dependencies, renewal information, and approved request route. |
| Household continuity | Dependents/pets, practical contacts, property/services, responsibility, continuity instructions, and applicable document references. |
| Wish/instruction | Subject, intended recipient, timing/context, visibility, revision, and distinction from legally established authority. |

Full bank numbers and government identifiers are not required for plan setup. Any sensitive data later supplied is masked by default and omitted from routine previews, notifications, analytics, and logs.

## 7. Functional requirements — access and handoff

### Sharing policy

V1 uses explicit sharing while the owner can consent. Records are private by default. An owner grants selected recipients access to selected records and the plan context those records need. The recipient accepts, the owner confirms identity and scope, and the recipient rehearses access. New record categories are not silently added to old grants.

Event activation does not expand permissions. Previously authorized recipients continue to use their grants after an event; the product does not require the unavailable owner's phone to approve every reading session. A person without an existing grant can work from information they independently supply, but cannot use death-reporting or support recovery to unlock the owner's private records.

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| ACCESS-01 | P0 | Separate account identities. | Every helper uses their own account. Owner credentials are never the normal handoff mechanism. |
| ACCESS-02 | P0 | Show invitation states accurately. | Invited, accepted, owner-confirmed, and rehearsal-complete are distinct. Expired/revoked invitations grant no access. |
| ACCESS-03 | P0 | Apply permissions to all representations. | An attachment, search result, export, task preview, cached summary, and notification cannot expose a record outside the user's grant. |
| ACCESS-04 | P0 | Separate collaboration from record access. | Assigning a task requests only the records required for it; assignment alone cannot disclose private source material. |
| ACCESS-05 | P0 | Revoke future access. | Revocation invalidates sessions/tokens for that grant and future downloads. The owner is told that already exported copies cannot be remotely recalled. |
| ACCESS-06 | P0 | Recover a recipient's own account safely. | Recovery uses the recipient's established methods and recovery material. Support cannot turn recipient-account recovery into an owner-record access grant. |
| ACCESS-07 | P0 | Survive loss of the owner's device. | A confirmed recipient can access already shared online records from their own replacement device without receiving a code on the owner's phone. |
| ACCESS-08 | P0 | Support multiple owners and affected people. | A household case can link separately permitted plans; consent and tasks remain attributable to each person. One partner's death does not unlock the other's private material. |
| ACCESS-09 | P0 | Audit sensitive access. | Record actor, action, record/category, time, permission basis, and outcome for access, sharing, export, and permission changes without logging document contents. |

Operational account disputes can temporarily restrict affected access for review; support must preserve evidence and notify eligible parties. Support staff have no unrestricted document-browsing interface.

## 8. Functional requirements — response workspace and task engine

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| CASE-01 | P0 | Start living-emergency or death response. | Event type, affected person, reporter, known date/location, existing preparation, and relevant roles are recorded; uncertainty is allowed. |
| CASE-02 | P0 | Generate applicable work from maintained rules. | Event, known records, roles, employment, enrolled dependents, jurisdiction, and completed work determine tasks. Unknown facts produce discovery tasks, not fabricated eligibility. |
| CASE-03 | P0 | Prioritize action without flooding the user. | Show at most three suggested next actions, each with a reason. The complete work list remains available by category and status. |
| CASE-04 | P0 | Track ownership and handoff. | Tasks have an assignee, acceptance/decline state, fallback coordinator, and last update. Unaccepted assignments remain visible to the coordinator. |
| CASE-05 | P0 | Support prerequisites and parallel work. | Separate required prerequisites from helpful preparation. A missing document does not block a call or an application process whose source permits starting without it. |
| CASE-06 | P0 | Maintain interaction history. | Users can record contact attempts, institution contacts, case references, received instructions, submissions, receipts, and follow-up dates. |
| CASE-07 | P0 | Identify deadline basis. | Store source, trigger, trigger date, rule version, calculated date, timezone/date convention, and verification category. A personal target date is labeled differently from an institutional deadline. |
| CASE-08 | P0 | Handle missing and conflicting evidence. | Missing-data tasks and disputed values are visible. The product preserves alternatives and identifies which institution must resolve the conflict. |
| CASE-09 | P0 | Correct the situation without destroying history. | Changing event type or correcting a date previews affected tasks and deadlines; user confirms changes. Existing submissions and evidence are retained. |
| CASE-10 | P0 | Support exceptions and undo. | User can mark not applicable, defer, reopen, or undo task completion with a recorded reason. Reopening does not claim an external action was reversed. |
| CASE-11 | P0 | Preserve case history and exports. | Case can be exported or archived with pending items explicitly identified. No silent removal of incomplete claims. |
| CASE-12 | P0 | Prevent duplicate effects. | Retrying an invitation, upload, assignment, or future integration request does not create duplicate records or external actions. Concurrent changes preserve the losing edit for resolution. |

### Task contract

Every actionable task contains: purpose; applicable situation; responsible role; official contact/action route; required and optional information; associated records/documents; prerequisites; source and review date; deadline basis if applicable; current state; assignee; history; and a definition of completion.

General task states are **not started, in progress, waiting on someone, blocked, completed, not applicable, deferred**. Institution-specific outcomes are tracked separately. An upload, prepared package, or clicked link never automatically marks an external claim or transfer complete.

## 9. Employer benefits and insurance requirements

### Benefit-specific behavior

| Benefit | Living emergency/incapacity | Death response |
| --- | --- | --- |
| LTD and other recorded disability coverage | Find applicable certificate, administrator, claim procedure, work/medical evidence, elimination-period terms and representative requirements. | Check existing claims, unpaid amounts, and any contract-specific survivor provision. Never describe LTD generically as a life payout. |
| Basic/supplemental life | Preserve coverage and beneficiary records; surface relevant contractual provisions only with supporting evidence. | Start employer/private-carrier claim route, obtain current coverage and beneficiary verification, create separate claimant records. |
| AD&D | Determine whether the reported event and applicable contract warrant inquiry; organize requested evidence. | Add accident-specific investigation/evidence tasks when relevant. Neither sudden death nor possession of a policy proves a covered accident. |
| Health, vision, dental | Find member/provider information, coverage and claims routes; coordinate relevant representative requests. | Determine survivors' coverage-end dates, continuation options, notices, elections, and premiums separately. |
| Retirement and other recorded benefits | Retain administrator and governing records. | Generate administrator inquiries and applicable survivor-benefit work without assuming the insurance beneficiary is also the retirement beneficiary. |

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| BENEFIT-01 | P0 | Distinguish evidence categories. | Offered, user-reported enrolled, documented enrollment, employer/carrier-confirmed coverage, and insurer decision remain separate. |
| BENEFIT-02 | P0 | Represent the employee's actual history. | Employment, leave, retirement, termination, coverage changes, and relevant dates can coexist. Current employment is not assumed from an old document. |
| BENEFIT-03 | P0 | Separate claimants and entitlements. | Each beneficiary has their own claimant record, forms, evidence access and outcome. A helper cannot view another claimant's private tax or payment data through a shared case. |
| BENEFIT-04 | P0 | Assemble a claim/request package. | User selects applicable documents and factual values, reviews a recipient-specific manifest, resolves missing required items, and exports a package or follows the supported provider handoff. |
| BENEFIT-05 | P0 | Reuse facts without signing for someone. | Identity, dates and contact details can be reused in drafts. Signatures, declarations, beneficiary choice, consent and payment instructions require the actual permitted signer. |
| BENEFIT-06 | P0 | Track claim lifecycle honestly. | Distinguish preparing, submitted, acknowledgment received, more information requested, decision received, payment pending, paid, appealed, withdrawn and closed. Each externally meaningful change identifies source/evidence or is labeled user-reported. |
| BENEFIT-07 | P0 | Separate coverage continuation clocks. | Death/event, coverage loss, notice, election and payment dates are distinct. No universal 60-days-from-death rule. |
| BENEFIT-08 | P0 | Find missing policies. | Where appropriate, provide official locator/employer inquiry tasks and explain that a locator request may not yield a response or complete inventory. |
| BENEFIT-09 | P0 | Preserve applicable forms and versions. | Every generated checklist/package identifies the selected provider form/version and review date. A source change flags affected unfinished packages for recheck. |

Potential coverage amounts are displayed with their evidence category. The product does not total unconfirmed coverage into an expected household payout.

## 10. Digital estate requirements

Digital affairs are a release capability, not a notes field. Personal profiles, cloud data, websites, domains, subscriptions, and organization accounts have different outcomes and permissions.

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| DIGITAL-01 | P0 | Inventory accounts and assets by type. | Distinguish personal profile, email/cloud identity, domain, hosting, organization Page/admin role, subscription and other asset. Records can be linked. |
| DIGITAL-02 | P0 | Record owner intent per asset. | Preserve, retrieve permitted data, continue permitted administration, transfer eligible asset, memorialize, close/delete, or undecided. A loved one's proposed change is attributed separately from the owner's recorded wish. |
| DIGITAL-03 | P0 | Record actual preparation status. | “Recorded in this app,” “provider designation reported,” and “designation evidence supplied” are distinct. An app invitation does not configure Apple, Google, or another provider. |
| DIGITAL-04 | P0 | Model access dependencies. | Account can depend on email, phone, device, password manager, administrator, domain, hosting or billing. Relevant dependencies appear before a closure/deletion handoff. |
| DIGITAL-05 | P0 | Expose only documented provider outcomes. | Google data request, Apple Legacy access, X deactivation, LinkedIn memorialization/closure, and GoDaddy estate-access workflows reflect their reviewed sources. No blanket “transfer social account” action. |
| DIGITAL-06 | P0 | Resolve preservation before closure. | If content retrieval is requested, account closure is blocked in the product's recommended sequence until resolved or explicitly overridden with a recorded reason and consequence. |
| DIGITAL-07 | P0 | Separate website components. | Domain, hosting, email, content, business admins and billing have distinct tasks and completion records. Domain movement cannot complete the others. |
| DIGITAL-08 | P0 | Track platform evidence and review. | Required ID/death/authority/key requirements are provider-specific. Outcomes remain pending until the user supplies the provider response. |
| DIGITAL-09 | P0 | Handle unverified platform support safely. | Instagram/TikTok and any unreviewed provider receive inventory, wishes, preservation/dependency work and a clearly labeled official-support handoff; no unsupported feature or transfer promise is displayed. |
| DIGITAL-10 | P0 | Protect private keys and credentials. | Store a reference to the owner's selected recovery arrangement rather than requiring passwords, master passwords, or seed phrases. Sensitive legacy-key documents can be separately permissioned. |

**Supported catalog at launch:** Google, Apple, Microsoft, X, LinkedIn personal profiles, LinkedIn organization-role continuity, GoDaddy domains/accounts, and Verizon mobile-account continuity using the reviewed procedures. Facebook receives historical-scope information and an official-support handoff until current detailed instructions are verified. Catalog support does not imply an API integration or successful access grant.

## 11. Documents, information quality, and exports

| ID | Priority | Requirement | Acceptance criteria |
| --- | --- | --- | --- |
| DOC-01 | P0 | Upload common evidence. | PDF, JPEG and PNG up to 20 MB/file; resumable retry on unreliable networks; file type validation and malware screening. Failed uploads are never shown as complete. |
| DOC-02 | P0 | Keep originals separate from working copies. | Source document remains unchanged; user can attach annotations/corrections as separate records. |
| DOC-03 | P0 | Identify proof type. | Distinguish a photo/copy stored in the app from an original, certified record, signed form, or institution-accepted submission. |
| DOC-04 | P0 | Preview disclosure. | Before an export, show recipients/purpose, included files and fields, omitted private material, missing items, and package timestamp. |
| DOC-05 | P0 | Produce useful portable output. | Human-readable PDF summary plus selected original attachments and a manifest in a downloadable archive. Include contacts, pending work and source references. No proprietary viewer is required. |
| DOC-06 | P0 | Preserve evidence links. | Task history references immutable document versions; replacing a file cannot rewrite what was submitted historically. |
| DOC-07 | P0 | Search within permission scope. | Search record metadata and user-supplied notes; a restricted document's existence/content cannot leak through results. Document-content search is not a launch dependency. |

Templates use recorded facts and selected source instructions. Generative AI is not required for any release-critical journey. No language model supplies eligibility, legal authority, institution confirmation, or invented deadline values.

## 12. Integration feasibility and delivery contract

### Capability assessment

| Action | What research supports | Launch behavior |
| --- | --- | --- |
| Prepare insurer claim paperwork | Insurers publish forms and specific employer/beneficiary processes. These support preparation; they do not establish a universal third-party submission API. | Checklist, selected documents, request draft/package, official submission handoff, recorded receipt/outcome. |
| Integrate employee-benefit administration | MetLife documents benefits-administration API partnerships. This does not establish access for this application to survivor claim submission or status. | No integration dependency or claimed carrier connection. |
| Obtain government survivor benefits | SSA documents its application routes and evidence requirements. No supported public third-party filing integration has been established by this research. | Application preparation and official contact route; user records agency response. |
| Settle or transfer bank accounts | Banks document ownership/authority review and estate-servicing procedures. A general account-data or payment API does not establish estate authority. | Account references, evidence checklist, institution handoff and follow-up. No movement of funds. |
| Access/memorialize/close online accounts | Providers document different request processes and limitations; X expressly refuses survivor access. No universal deceased-account transaction API has been established. | Provider-specific request preparation and handoff. No credentials, auto-login or ownership promise. |
| Obtain domain/account access | GoDaddy documents an estate-administrator review process. It does not establish automatic acceptance or universal transfer rights. | Component inventory, authority/document preparation, official review handoff, recorded outcome. |

Feasibility claims above are deliberately limited to the researched operation and provider. “Not established” is not “technically impossible.” Unsupported execution is outside launch scope, not a request for the founder to guess.

### Contract for enabling any future direct action

A specific external capability can be enabled only after all of the following are demonstrated:

1. Official API or written partner permission covers the exact action, account type, region, user role, and product use case.
2. Required commercial access and production credentials are approved; sandbox availability alone is insufficient.
3. Identity, representative authority, user consent, signatures and institution-required disclosures are accepted through that channel.
4. The product exposes exact payload/recipient/action confirmation and performs no broader operation.
5. Retries are idempotent, errors are recoverable, and an authoritative external reference/outcome is recorded.
6. Status synchronization and reconciliation distinguish accepted, processing, rejected, failed and completed.
7. Users retain a supported manual route when the integration is unavailable or does not support their case.
8. Data handling, support responsibility, deletion and audit requirements are reviewed before production enablement.

## 13. Content and guidance operations

Every actionable procedure is a versioned catalog entry with provider, action, jurisdiction, applicable account/plan type, event type, source URLs, reviewed date, reviewer, required roles/evidence, steps, deadline rules, permitted outcomes and known limitations.

- First-party institutional and government sources take precedence over secondary summaries.
- A content operator prepares an update; a second reviewer approves high-impact changes to authority, deadlines, disclosure or irreversible actions.
- High-impact procedures are reviewed at least every 30 days; other procedures at least every 90 days. User reports and detected source changes trigger earlier review.
- After a failed/stale review, the affected detailed instructions are withdrawn from new recommendations; the official-support route and record remain available. Previously generated packages are flagged for recheck.
- Existing cases preserve the old procedure version and show the reason for a relevant update. Historical submissions are not rewritten.
- A provider response received by a family is case-specific evidence, not an automatic global policy update.
- General targets such as “follow up next week” are distinguished from documented filing/election/payment deadlines.

## 14. Data and state requirements

### Core entities

**User, Person, HouseholdLink, Plan, Record, RecordVersion, DocumentVersion, Contact, Grant, Invitation, Rehearsal, EventCase, DeclaredRole, Task, TaskDependency, Assignment, InstitutionRequest, SubmissionPackage, ExternalReference, Deadline, Interaction, ProcedureVersion, AuditEvent.**

Every case action identifies the affected person. Records and documents identify their owner, uploader, permitted recipients and version. A role claim records its evidence and which institution, if any, has accepted it; it does not become globally “verified authority.”

### Important transitions

- **Grant:** invited → accepted → owner-confirmed → active; owner can revoke. Rehearsal completion is separately recorded.
- **Case:** active → ongoing follow-up → resolved → archived; recovery, death, or correction creates a versioned event change.
- **Package:** draft → reviewed → exported/handed off → user-reported submitted → receipt recorded. Exported does not mean submitted.
- **External outcome:** reported/submitted → acknowledged → additional information/decision → final outcome, with evidence category and date.
- **Procedure:** draft → reviewed → published → superseded/withdrawn. Active cases pin the version used.

Deleting a source record must identify dependent cases and evidence. It may remove future display while retaining only the minimum separately authorized evidence necessary for a case; deletion scope and retention are previewed explicitly. A recipient's independently contributed case records do not silently become the affected person's private plan property.

## 15. Privacy, security, and continuity requirements

| ID | Requirement | Release acceptance |
| --- | --- | --- |
| SEC-01 | Authenticate account access and protect sensitive actions. | Support passkey-based authentication and a recovery mechanism; require fresh authentication for grants, exports, recovery changes and deletion. Device biometrics protect locally saved sensitive content. |
| SEC-02 | Enforce authorization on the server. | Automated tests cover cross-user, cross-household, revoked-grant, attachment, search, export and case-sharing access. No client-only permission enforcement. |
| SEC-03 | Encrypt data and restrict service access. | Modern TLS in transit; encrypted storage and managed keys with restricted service roles. Do not market the service as end-to-end encrypted or zero-knowledge unless that architecture is actually delivered and verified. |
| SEC-04 | Keep sensitive data out of telemetry. | No document text, account numbers, health details, keys, identity documents or names in analytics/crash payloads. Notifications contain generic task references. |
| SEC-05 | Make support access explicit and narrow. | Support can inspect operational metadata; document access requires a narrowly scoped, time-limited authorization and audit event or an applicable legal process. |
| SEC-06 | Respect deletion and retention. | User can export then request deletion. Active access is removed promptly; primary-store deletion target is 30 days and backup expiry within 90 days, subject to clearly disclosed legal preservation obligations. |
| SEC-07 | Avoid confidentiality overclaims after export. | Preview explains that downloaded/exported copies leave revocable app control. Export itself requires current authorization. |
| SEC-08 | Preserve usable access during an incident. | Users can export a portable plan and case record at any time. Recovery procedures are exercised before launch; support does not bypass sharing permissions during an incident. |
| SEC-09 | Keep adversarial event reports from becoming access grants. | Reporting a death, matching a person's identity, uploading a certificate, or claiming executor status cannot independently unlock private owner records in V1. |

### Offline emergency summary

Offline saving is deliberate and per device. The user selects already permitted essential contacts, selected coverage references, document locations and instructions. The app shows what is saved, its update date, and the fact it may be stale. Documents beyond the selected scope are not cached automatically. The cache is encrypted and protected by device authentication; signing out removes app-managed cached data.

Revocation cannot be guaranteed to erase an offline device before it reconnects. On reconnection the app checks grants before refreshing or continuing sensitive access and removes revoked cached records. This limitation is stated at the point the owner grants offline availability.

## 16. Experience requirements

- The response experience begins with the affected person, situation, immediately useful information and next work; preparation and active response are visibly distinct contexts.
- Navigation gives access to the plan/information, active work, people, documents and wishes without requiring a marketing-style home screen.
- Missing information can be saved and revisited. No long mandatory onboarding before useful contacts or tasks become available.
- Contact actions make calling or opening the official channel easy and return the user to the related task/history.
- Supporting information is progressively disclosed; the main task explains the next action, responsible role, prerequisites and completion evidence.
- No countdown is shown without a known trigger and source. No urgent styling is applied merely because a task exists.
- Copy distinguishes “you recorded,” “document says,” “provider confirmed,” and “decision received.”
- Users can pause, leave, and resume without losing entered work or being pressured to describe feelings.
- Conform to WCAG 2.2 AA where applicable, support VoiceOver/TalkBack, OS text scaling to 200%, logical focus order, text labels beyond color, and touch areas of at least 44 pt on iOS/48 dp on Android.
- The supplied Ink wash palette is a visual input, not permission to sacrifice contrast. Typography, components and final visual design follow this PRD; rejected screen concepts are not implementation references.

## 17. Reliability and performance targets

| Area | Target and measurement |
| --- | --- |
| Core availability | 99.9% monthly for authentication, permitted-plan read and case read/write, measured at service boundary. Third-party availability is reported separately. |
| Read responsiveness | p95 plan summary and next-task responses below 2 seconds server-side for a 100-record plan under normal load; first useful content below 3 seconds in the defined mobile test profile. |
| Save behavior | Explicit saved/pending/failed states; recoverable local drafts; no silent loss on network interruption or app restart. |
| Upload | A 20 MB supported document either completes with confirmation or remains resumable/retryable with no false success state. |
| Reconciliation | Permission changes and concurrent edits are checked before sensitive exports/actions. Conflict handling never silently overwrites another person's evidence. |
| Recovery | Recovery point objective ≤24 hours and recovery time objective ≤24 hours for service disaster; backup restoration exercised before launch. |
| Scale baseline | Validate 1,000 records, 250 documents and 500 tasks per plan/case without broken navigation, export, or permission enforcement. |
| Accessibility | No release-critical journey requires sight, fine motor precision, or text smaller than the supported OS accessibility settings allow. |

Performance test profile: a representative midrange iOS/Android device, 10 Mbps network with 100 ms latency, cold and warm launches, and the reference data volumes above. Targets are release requirements, not measured claims about an existing application.

## 18. Measurement

Primary product measure: **a responding person can complete the next applicable preparation/handoff step with the right information and record the outcome without assistance from the unavailable plan owner.**

| Measure | Definition | Initial release target |
| --- | --- | --- |
| Successful recipient handoff | Confirmed recipient independently locates a contact/document and completes rehearsal. | ≥90% of attempted rehearsals in the release study. |
| Time to useful information | Time from recipient entry to locating the selected essential contact or document location. | Median ≤2 minutes; p90 ≤5 minutes in representative task testing. |
| Task-path comprehension | Participant correctly identifies next action, responsible role and required evidence for a scenario. | ≥90% across the launch scenario set. |
| Supported package accuracy | Review finds the selected procedure, required items, recipient and facts correctly represented. | 100% of mandatory release fixtures; no critical misrouting. |
| Permission isolation | Unauthorized cross-user/case/record access succeeds. | Zero in release security tests. |
| Source integrity | Actionable catalog item includes valid scope, evidence, owner and review date. | 100% of published launch procedures. |
| Outcome integrity | An external action is shown as confirmed solely from a click/export or an unsupported inference. | Zero in release fixtures. |

These are evaluation targets, not observed results. External insurer approval rates, benefit dollars and estate duration are not attributed to the product without an appropriate study. Analytics measure flow states using pseudonymous identifiers and do not collect the underlying private content.

## 19. End-to-end release acceptance scenarios

| ID | Scenario | Required result |
| --- | --- | --- |
| A01 | Owner records only employer and HR contact. | Plan saves; recipient can use permitted contact; unknown coverage becomes inquiry work. |
| A02 | Recipient accepts but owner has not confirmed. | No record access; readiness remains incomplete. |
| A03 | Owner confirms a limited grant. | Recipient sees exactly the permitted records and attachments; no private search/export leakage. |
| A04 | Owner loses their phone. | Confirmed recipient uses their own account to access existing grants. |
| A05 | Loved one starts without a prepared plan. | Discovery workspace provides useful initial work without implying access to an existing owner's private plan. |
| A06 | Owner's benefits brochure lists supplemental life but election is unknown. | Coverage remains unconfirmed; no payout promise; employer verification task appears. |
| A07 | Several beneficiaries and one minor are recorded. | Separate claimant work and access; minor-representation requirements come from the selected procedure. |
| A08 | Death may have been accidental and reports are pending. | AD&D inquiry is separate; requested evidence can remain pending; no eligibility assumption. |
| A09 | SSA claimant lacks a marriage document. | Product preserves the source's ability to initiate contact/application without waiting for all documents. |
| A10 | Survivor receives continuation notice after coverage loss. | Election/date handling uses the applicable documented trigger; payment remains a separate task. |
| A11 | Living disability case later becomes a death case. | History and prior submissions remain; newly relevant tasks appear with reviewed dependencies. |
| A12 | A claimed executor uploads a death certificate. | No automatic private-plan disclosure; product role is not presented as globally institution-verified. |
| A13 | Google data retrieval and account closure are both intended. | Preservation dependency is visible and closure is sequenced after retrieval resolution or explicit informed override. |
| A14 | Apple Legacy Contact is recorded without the access key. | Readiness shows the missing prerequisite; product does not promise password/passkey recovery. |
| A15 | Family wants control of an X account. | Supported route is the documented removal request; survivor login/transfer is not offered. |
| A16 | A personal profile also administers an organization Page. | Personal-profile and organization continuity tasks remain separate. |
| A17 | GoDaddy domain movement is confirmed. | Hosting, email, billing and content tasks remain unfinished unless separately resolved. |
| A18 | A platform's current detailed procedure is unverified. | No fabricated checklist or automation; inventory/dependency work and official support route remain available. |
| A19 | A helper declines or ignores an assignment. | Coordinator retains visibility and can reassign without losing context. |
| A20 | Source procedure changes while a package is being prepared. | Package is flagged for recheck; existing submission evidence is preserved. |
| A21 | Owner revokes a recipient with an offline copy. | Online access is revoked; cache is removed on reconnection; prior offline/export limitation is represented accurately. |
| A22 | Both household partners are affected. | Fallback recipients use their existing separate grants; one person's event does not unlock the other person's private plan. |
| A23 | Upload fails and the app is restarted. | Draft work remains and upload is retryable; no false completed attachment. |
| A24 | User exports a claim package. | Exact manifest and disclosure scope are reviewed; export does not mark the claim submitted or paid. |
| A25 | Screen reader and 200% text scaling are used. | Complete preparation, recipient access, case activation, task handoff and export journeys remain operable. |
| A26 | State-specific instructions are unsupported. | Product gives the appropriate contact/discovery route and does not invent deadlines or authority requirements. |
| A27 | Date of death is corrected after submissions. | User sees affected tasks/deadlines, prior values and evidence; no silent recalculation of historical submissions. |
| A28 | A claimant reports payment received. | Record identifies user report and evidence; unrelated claims are not automatically completed. |

## 20. Release sequence and gates

### Increment 1 — Preparation and usable handoff

Deliver structured plan records, documents, explicit sharing, recipient confirmation/rehearsal, exports and permission auditing. Gate: A01–A04, A12, A21–A23 and core accessibility/security requirements pass.

### Increment 2 — Active response and benefits work

Deliver prepared/unprepared case entry, living/death distinctions, maintained task rules, assignments, benefits-specific workflows, submission preparation, dates and outcome history. Gate: A05–A11, A19–A20, A24, A26–A28 pass; all published procedures have reviewed scope and sources.

### Increment 3 — Digital affairs and production readiness

Deliver the stated digital catalog, preservation dependencies, organization/website component handling, offline emergency summary and complete reliability/accessibility checks. Gate: A13–A18 and A25 pass, disaster recovery is exercised, permission tests pass, and the complete J1–J5 journeys succeed on both mobile platforms.

All three increments constitute the first production release. These are delivery units, not separate promises of complete public products. No calendar estimate is asserted before implementation planning and staffing.

## 21. Evidence and traceability

| Requirement family | Research basis |
| --- | --- |
| Preparation, emotional/administrative burden and household work | [Research register R01–R04](docs/research/evidence-register.md#r01); [31-task work map](docs/research/after-death-work-map.md). |
| Coverage, claimants and insurance evidence | [MetLife claim process](https://www.metlife.com/support-and-manage/file-a-claim/); [Pacific Life actual employer/beneficiary packet](https://www.pacificlife.com/content/dam/paclife/wbd/public/Life-Employer-Claim-Package.pdf); register R05–R10. |
| Survivor applications and authority | [SSA application evidence](https://www.ssa.gov/forms/ssa-10.html); [Bank of America estate process](https://www.bankofamerica.com/signature-services/estate-services/); register R11–R13, R22, R24–R29, R36. |
| Digital preservation and provider-specific outcomes | [Google deceased-user requests](https://support.google.com/accounts/troubleshooter/6357590); [Apple Legacy Contact](https://support.apple.com/en-us/102631); [X deceased-account procedure](https://help.x.com/en/rules-and-policies/contact-x-about-a-deceased-family-members-account); [LinkedIn policy](https://www.linkedin.com/help/linkedin/answer/a1336663/memorialize-or-close-the-account-of-a-deceased-member); register R14–R21, R37–R38. |
| Website component distinction | [GoDaddy estate access](https://www.godaddy.com/help/how-to-gain-access-to-domains-or-accounts-after-account-holders-death-8356); [domain transfer limitations](https://www.godaddy.com/help/transfer-my-domain-to-another-godaddy-account-822). |
| Integration boundary | [MetLife Benefits Bridge](https://www.metlife.com/business-and-brokers/broker-resources/metlife-benefits-bridge/) documents administration partnerships; the reviewed claim and platform procedures do not establish a production transaction integration for this application. |
| Competitive context | Register R30–R35 documents existing overlap. This PRD makes no “first,” exclusive-category, or validated-market-advantage claim. |

The source review establishes procedural constraints and available public routes. The release choices, access model, technical targets and measurement gates in this PRD are specified product requirements, not claims that the sources prescribe this implementation or that testing has already occurred.
