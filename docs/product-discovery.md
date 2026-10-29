# If Something Happens — product discovery record

Date: October 29, 2026  
Status: historical discovery record. The [PRD](../PRD.md) now supplies the working release decisions, requirements, and acceptance criteria; the unresolved discussion below is retained as history.

## 1. Origin and established intent

The idea arose when the founder and their spouse discussed private insurance policies, bank accounts, and employee benefits. The employee benefits included long-term disability (LTD), accidental death and dismemberment (AD&D), supplemental life, health, vision, and dental insurance. The conversation exposed a practical gap: a loved one may not know what exists, whom to call, which paperwork is required, what may be payable, or how to begin.

The intended product is a mobile application called **If Something Happens**. Its intended beneficiaries include spouses, partners, children, and caregivers facing a loved one's emergency or possible death. The founder also explicitly identified web and social-media account access and transfers as critical.

The desired outcome is an organized plan and the information needed to act during a difficult period, including benefits, insurance claims, contacts, and personal wishes.

The founder has not approved an MVP, architecture, release mechanism, subscription model, jurisdiction, or visual design. An earlier concept's presentation of situation, people, next task, contact, ownership, and supporting tasks was liked; its appearance was rejected. That feedback does not approve a complete product workflow.

## 2. Research findings that change the product discussion

| Finding | Evidence | Consequence to investigate |
| --- | --- | --- |
| Families face administrative and emotional burdens together. | A 2024 UK qualitative study analyzed responses from 1,133 bereaved adults and identified difficult initial contact, paperwork, timelines, and organizational failures. [R01](research/evidence-register.md#r01) | Investigate whether reducing repeated explanations and tracking unresolved interactions matters more than adding another information repository. UK findings are not a U.S. prevalence estimate. |
| Knowing a benefit exists does not establish actual coverage or entitlement. | Employer claim packets require coverage verification and current beneficiary records. [R05–R07](research/evidence-register.md#r05) | Distinguish offered benefits, actual enrollment, applicable terms, named beneficiaries, and insurer determinations. |
| Several people may have different responsibilities. | A beneficiary claims insurance; an estate representative manages estate matters; a platform applies its own access rules. [R06, R11, R19](research/evidence-register.md#r06) | Investigate the roles separately rather than using “trusted person” for every kind of authority. |
| Actions have dependencies and can remove future options. | Google warns that closure prevents later content requests; domain movement does not move connected hosting/email products. [R14, R21](research/evidence-register.md#r14) | Investigate ordering, preservation decisions, and unfinished prerequisites, not just a list of accounts. |
| Some readiness work must happen while the owner is alive. | Apple requires a pre-created legacy access key; emergency-access services require accepted/confirmed arrangements. [R16, R23](research/evidence-register.md#r16) | Investigate what constitutes a usable handoff and how a recipient knows it exists. |
| Information access does not confer legal or institutional authority. | Banking, postal, insurance, and platform procedures request different evidence. [R11, R19, R26](research/evidence-register.md#r11) | Investigate how to explain roles and document requirements without promising authority the app cannot grant. |
| This is an existing product category with substantial overlap. | Empathy, Everplans, Trustworthy, and GoodTrust document preparation, sharing, benefits organization, or post-loss support. [R30–R35](research/evidence-register.md#r30) | A distinctive unmet need must be demonstrated. “A vault plus checklist” is not an established competitive gap. |

## 3. People and situations to investigate

These are research segments, not finished personas.

| Person or situation | What needs to be understood |
| --- | --- |
| Person preparing their own information | What they can find, what they avoid recording, what changes over time, and what they are comfortable sharing. |
| Surviving spouse or partner | What they know already, household continuity, beneficiary status, and differences between marriage, partnership, account ownership, and legal appointment. |
| Adult child or caregiver | Whether they know the institutions, can locate documents, and have authority for the particular action. |
| Executor, administrator, trustee, or professional helper | Which responsibilities belong to them, which evidence they need, and how family members coordinate without exceeding their roles. |
| Household with minor children or other dependents | Immediate continuity of care, existing legal arrangements, and separate management of inherited money. |
| Owner who is alive but unavailable or incapacitated | Consent, representative authority, disability/leave, and access during temporary incapacity. This remains a separate investigation from death administration. |
| Family with little or no preparation | Whether useful assistance is possible without an existing account, known inventory, or accepted invitation. |

## 4. Questions the evidence supports investigating

1. **Finding information:** Can the loved one discover the institutions, benefits, accounts, wishes, and people that matter, including records that were never entered?
2. **Understanding relevance:** Can they distinguish a possible benefit from confirmed coverage and determine the right institution to ask?
3. **Establishing authority:** Can they identify who can perform a task and the evidence that organization requires?
4. **Taking action:** Can they obtain the right instructions, forms, contact route, and submission requirements?
5. **Following through:** Can they tell whether something was merely reported, formally claimed, received, incomplete, approved, paid, transferred, or closed?
6. **Maintaining continuity:** Can they preserve household services, dependent care, records, and digital assets while other work remains unresolved?

These are problem statements. They do not decide which capabilities the first release should implement.

## 5. Open product decisions, in order of dependency

| Decision | Why it changes the product | Current status |
| --- | --- | --- |
| Initial geography and legal scope | Determines institutions, forms, terminology, authority, and deadlines. | U.S. research assumption only; no state selected. |
| First supported situation | Death, living incapacity, and emergency recovery involve different actors and evidence. | Both emergencies and death are established long-term intent; release sequence undecided. |
| Starting condition | An existing prepared plan and an unprepared survivor have different discovery and access needs. | Neither path selected as the first focus. |
| Primary user's role | A spouse, beneficiary, caregiver, and estate representative cannot be treated as interchangeable. | Audience named; first supported role unresolved. |
| Product's level of responsibility | Organizing information, explaining procedures, coordinating work, submitting claims, and providing human assistance are different commitments. | Unresolved; research does not justify assuming automated filing. |
| Information sharing and release | What is shared while alive, what changes at death, who initiates access, and how mistaken requests are handled. | No mechanism selected. |
| Guidance provenance and maintenance | Claim instructions and platform policies vary and change. | Ownership of verification and updates unresolved. |
| Sustainable access | Recipients may need the information during subscription lapse, service failure, or loss of the owner's device/email. | Business and continuity model unresolved. |

## 6. Hypotheses requiring direct validation

- The hardest gap may be converting scattered records into a correctly ordered, role-appropriate process, rather than storing more records.
- Employer-benefit discovery may be especially valuable where the surviving person cannot use an employee portal and does not know actual elections.
- A recipient may believe they are prepared after receiving an invitation even though they cannot independently locate or access the information.
- Digital continuity may require coordination across email, phone numbers, authentication, cloud data, domains, and business administrators.
- People may need useful help even when the deceased never prepared a plan.

None of these statements is an interview finding, validated demand, or approved feature.

## 7. Evidence needed before an MVP decision

Use recent real cases and de-identified artifacts where participants choose to provide them. Do not ask participants to submit credentials or sensitive financial records.

| Investigation | Questions to resolve | Useful evidence |
| --- | --- | --- |
| Conversations with people who handled a death | What happened first? What was unknown? Where did progress stop? Which tasks were repeated or missed? | Reconstructed chronology, actual institutions contacted, redacted request lists, and points of delay. |
| Conversations with people preparing a household | What information can they actually assemble? What would they share, with whom, and when? | Attempted inventory and explanations of omissions or reluctance. |
| Benefits-administrator review | What can a survivor obtain, from whom, and which records prove coverage and beneficiary status? | Current claim packets and representative employer procedures. |
| Estate-professional review in a selected jurisdiction | Which tasks belong to which roles, and what timing or sequencing cannot be generalized? | Reviewed task-map corrections and authoritative local sources. |
| Digital-account policy verification | Which account types, regions, and desired outcomes are supported? | Current official procedures; unresolved Instagram/TikTok routes remain explicitly open. |
| Existing-product evaluation | Can representative tasks be completed with current products, and where do they fail? | Observed task results rather than marketing comparison alone. |

## 8. Boundaries of this record

No original user interviews or product trials have been conducted. Published research, public instructions, and competitor descriptions are different evidence types. The task map is a research model; it is not personal legal, medical, or financial instructions and does not establish that every listed task applies to every household.

The next product discussion should resolve the first five decisions above against this evidence, then record the chosen scope and its rationale. A full PRD and screen design follow those decisions.
