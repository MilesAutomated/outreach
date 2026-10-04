# Business Proposal: Outbound AI Voice Agent Development & Deployment

### Chloride Exide Kenya | Automotive Batteries · Solar Products · Energy Storage

---

## 1. Title Block & Document Metadata

| Field | Detail |
| --- | --- |
| **Document Title** | Outbound AI Voice Agent: Development & Deployment Proposal |
| **Prepared For** | Dominic and Team, Chloride Exide |
| **Prepared By** | Kamunya Maina |
| **Business Lines in Scope** | Automotive Batteries (incl. Dial-a-Battery), Solar Products, Energy Storage / Inverters |
| **Engagement Model** | 30-day build and launch, within a 3-month onboarding engagement, followed by a monthly maintenance retainer |
| **Total One-Time Setup Investment** | **$4,000 USD (KSh 520,000)** |
| **Ongoing Maintenance** | **$100 USD / month (KSh 13,000)**, starting after the 3-month onboarding period |
| **Third-Party Usage Costs** | Paid directly by Chloride Exide (telephony, AI speech processing, SMS) |
| **Currency Basis** | USD is the contract currency. KES figures use a fixed reference rate of **130 KES = 1 USD** |
| **Document Status** | Final Draft: For Client Review & Sign-Off |
| **Version** | 1.0 |
| **Classification** | Confidential: Prepared exclusively for Chloride Exide |

---

## 2. Executive Summary & Business Objective

### 2.1 The Business Objective

Chloride Exide serves motorists, households and businesses whose products are bought rarely but matter a great deal when they fail. A flat car battery, an inverter fault or a solar system that underperforms all need a prompt, competent response. Leads that are not followed up go cold, and simple diagnostic questions take up support staff who could be working on complex cases.

The objective of this engagement is to deploy a **dedicated outbound AI voice agent** that:

1. **Follows up on leads and customers consistently** at a controlled pace of about **20 calls per working day**.
2. **Handles Tier-1 technical triage** for automotive batteries (including Dial-a-Battery qualification) and solar/inverter systems, using **only Chloride Exide–approved knowledge base material**.
3. **Passes complex cases to people** through a warm live transfer to staff, and books technician visits or sales consultations directly into company calendars.
4. **Records every interaction in the CRM.** The full transcript, a structured summary and disposition tags are written to the customer record as soon as each call ends.
5. **Confirms outcomes by SMS** with diagnostic links, Dial-a-Battery links and booking confirmations.

### 2.2 Design Principles

The scope has been deliberately limited so the system stays dependable, easy to audit and inexpensive to run:

| Principle | How It Is Applied |
| --- | --- |
| **Outbound only** | The AI agent only makes outbound calls. **No inbound AI agent is included.** Every inbound call bypasses the AI and is forwarded directly to Chloride Exide's human support team. |
| **Stateless per call** | Each call starts from the context supplied by the call trigger (CRM record and call list). Nothing is remembered between calls during a session. The CRM is the single system of record. |
| **SMS-only follow-up** | Automated post-call messages are sent **by SMS only**. Email sequencing and email campaigns are excluded. |
| **Approved content only** | Troubleshooting guidance is limited to documentation Chloride Exide has reviewed and approved. Anything beyond Tier-1 is transferred to a person. |
| **Transparent usage costs** | Chloride Exide pays third-party infrastructure costs directly at provider rates, with no markup. |

### 2.3 Commercial Summary

| Item | USD | KES (@130) |
| --- | --- | --- |
| Trial Deposit: due at signing (funds the 30-day build and Month 1 optimization) | $500 | KSh 65,000 |
| Milestone 2: due before Month 2 optimization, if Chloride Exide elects to proceed | $3,500 | KSh 455,000 |
| **Total One-Time Setup Investment** | **$4,000** | **KSh 520,000** |
| Maintenance Retainer: from Month 4 onward | $100 / month | KSh 13,000 / month |
| Third-Party Usage | Paid directly by Chloride Exide | Usage-based |

Chloride Exide's initial commitment is limited to **$500**. The decision to continue is made after the agent has been built, launched and tested against real call outcomes.

---

## 3. Detailed Scope of Work

### 3.1 Included Deliverables

| # | Deliverable | Description | Acceptance Criteria |
| --- | --- | --- | --- |
| D1 | **Outbound Follow-Up & Lead Engagement** | Scheduled outbound calls to customer and lead lists approved by Chloride Exide, paced at about **20 calls per working day (Monday–Friday)**. Call lists are pulled from the CRM or an approved list source. | Calls run within agreed calling windows, at the target pace, only to approved lists. |
| D2 | **Tier-1 Automotive Battery Triage** | Structured diagnostic questioning on common battery symptoms (e.g. slow cranking, no-start, warning lights, battery age). Includes **Dial-a-Battery qualification**: confirming vehicle details, location and urgency, then routing the customer to purchase or booking. | Agent responses match the approved knowledge base and qualification logic in UAT test scripts. |
| D3 | **Tier-1 Solar & Inverter Triage** | Structured guidance on common solar panel, inverter and energy storage questions (e.g. backup duration, charging behaviour, error indicators, basic checks), drawn only from approved Chloride Exide documentation. | Agent responses match approved documentation. Out-of-scope questions trigger a transfer or a booking. |
| D4 | **Warm Live Transfer to Human Staff** | Live call handoff to a designated Chloride Exide staff line when a query goes beyond Tier-1 logic or the customer asks for a person. The agent introduces the context before connecting where the telephony setup supports it. | Transfers connect successfully in testing for both triggers: complexity escalation and customer request. |
| D5 | **Calendar Booking Integration** | Real-time availability checks and direct booking of **technician visits** and **sales consultations** on designated company calendars. | Bookings appear on the correct calendar with customer details and call reference. |
| D6 | **Post-Call CRM Synchronization** | Immediately after each call, the system writes the **full conversation transcript**, a **structured summary**, and **disposition tags** (e.g. Qualified, Booked, Transferred, Callback Requested, Not Interested, No Answer) to the customer record. | 100% of completed test calls produce a correctly mapped CRM write-back. |
| D7 | **Automated Post-Call SMS** | Event-triggered SMS sent through Chloride Exide's SMS provider: diagnostic and self-help links, Dial-a-Battery order links, branch/location details and booking confirmations. | SMS delivered for each defined trigger in UAT, with approved message templates. |
| D8 | **Static Inbound Call Forwarding** | Telephony forwarding rules so that **all inbound calls go directly to Chloride Exide's human support team** with no AI involvement. | Test calls to inbound numbers reach the support desk with no AI interaction. |
| D9 | **Authorized Production Voice Clone** | A production voice model built from clean reference audio supplied by Chloride Exide, with **explicit written consent** from the voice owner. A professional stock voice is used until consent and audio are received. | Signed consent on file. Voice approved by Chloride Exide before go-live. |
| D10 | **Launch, Handover & Documentation** | Production launch, live monitoring during launch week, and a handover pack covering system overview, escalation contacts, disposition definitions and change-request process. | Handover pack delivered and walkthrough session completed. |
| D11 | **3-Month Optimization Program** | Month-by-month tuning of prompts, triage logic, transfer thresholds and SMS triggers based on real call outcomes (see Section 6). | Monthly performance review delivered. |

### 3.2 Explicit Out-of-Scope Exclusions

The following items are **not included** in this engagement. Any of them would need a separate written change request, with its own scope, timeline and pricing.

| Exclusion | Clarification |
| --- | --- |
| **Inbound Conversational AI Agent** | **Inbound AI is out of scope.** No inbound AI agent, conversational IVR, AI virtual receptionist or AI call answering will be built. All inbound calls bypass the AI completely and are forwarded statically to Chloride Exide's human support team. |
| **Email Marketing, Sequencing & Campaigns** | No automated emails, drip sequences, newsletters or email campaigns. **Post-call follow-up is SMS only.** |
| **Dynamic Cross-Call / In-Session Memory** | The agent does not build or update customer profiles in real time across calls. Context is supplied when each outbound call is triggered, and results are written to the CRM after the call. |
| **Tier-2+ Technical Support** | Advanced diagnostics, warranty adjudication, pricing exceptions, complaint resolution and anything not covered by approved documentation. These are transferred to staff. |
| **Payment Processing** | The agent does not take card, M-Pesa or other payments during calls. It may send an SMS link to an existing Chloride Exide ordering channel (e.g. Dial-a-Battery). |
| **Knowledge Base Authoring** | Chloride Exide supplies and approves all technical content. This engagement covers ingesting and structuring that content, not writing new technical documentation. |
| **CRM / SMS Platform Procurement or Re-Platforming** | Integration targets Chloride Exide's existing CRM, calendar and SMS provider. New licences, migrations or custom CRM development are excluded. |
| **High-Volume or Multi-Campaign Dialing** | Pacing is designed around about 20 calls per working day. A material increase in volume or additional campaigns would be scoped separately. |
| **Third-Party Usage Fees** | Telephony, AI speech processing and SMS carrier fees are paid by Chloride Exide and are not part of the setup or retainer fees. |
| **Unconsented Voice Cloning** | No voice will be cloned without explicit written consent from the voice owner and clean reference audio supplied by Chloride Exide. |

---

## 4. System Architecture & Routing Flow

### 4.1 High-Level Architecture

The telephony layer splits traffic at the edge into two separate paths. **Inbound** traffic never reaches the AI. **Outbound** traffic is started by the system and handled by the AI agent.

```
                         ┌───────────────────────────────────┐
                         │    TELEPHONY INFRASTRUCTURE       │
                         │  (Carrier / SIP Trunk / Numbers)  │
                         └─────────────────┬─────────────────┘
                                           │
             ┌─────────────────────────────┴─────────────────────────────┐
             │                                                           │
             ▼                                                           ▼
 ╔═══════════════════════════╗                         ╔═══════════════════════════════╗
 ║   PATH A: INBOUND CALLS   ║                         ║   PATH B: OUTBOUND CALLS      ║
 ║      (NO AI INVOLVED)     ║                         ║    (AI VOICE AGENT)           ║
 ╚═════════════╤═════════════╝                         ╚═══════════════╤═══════════════╝
               │                                                       │
               ▼                                                       ▼
 ┌───────────────────────────┐                         ┌───────────────────────────────┐
 │  Static Call Forwarding   │                         │  Call Trigger                 │
 │  Rule (carrier-level)     │                         │  • Approved call list (CRM)   │
 └─────────────┬─────────────┘                         │  • Customer context payload   │
               │                                       │  • Pacing: ~20 calls/day      │
               ▼                                       └───────────────┬───────────────┘
 ┌───────────────────────────┐                                         │
 │  CHLORIDE EXIDE           │                                         ▼
 │  HUMAN SUPPORT TEAM       │                         ┌───────────────────────────────┐
 └───────────────────────────┘                         │  Outbound AI Voice Agent      │
                                                       │  • Follow-up / lead engagement│
                                                       │  • Tier-1 battery triage      │
                                                       │    (Dial-a-Battery qual.)     │
                                                       │  • Tier-1 solar/inverter      │
                                                       │  • Approved knowledge base    │
                                                       └───────┬───────────┬───────────┘
                                                               │           │
                                     ┌─────────────────────────┘           └───────────┐
                                     ▼                                                 ▼
                     ┌───────────────────────────────┐               ┌───────────────────────────┐
                     │  Calendar Booking             │               │  Warm Live Transfer       │
                     │  • Technician visits          │               │  • Beyond Tier-1 logic    │
                     │  • Sales consultations        │               │  • Customer requests human│
                     └───────────────┬───────────────┘               └─────────────┬─────────────┘
                                     │                                             │
                                     └──────────────────────┬──────────────────────┘
                                                            ▼
                                            ┌───────────────────────────────┐
                                            │        CALL COMPLETED         │
                                            └───────────────┬───────────────┘
                                                            │
                                  ┌─────────────────────────┴─────────────────────────┐
                                  ▼                                                   ▼
                  ┌───────────────────────────────┐                   ┌───────────────────────────────┐
                  │  CRM SYNCHRONIZATION          │                   │  SMS FOLLOW-UP (SMS ONLY)     │
                  │  • Full transcript            │                   │  • Diagnostic / self-help link│
                  │  • Structured summary         │                   │  • Dial-a-Battery link        │
                  │  • Disposition tags           │                   │  • Booking confirmation       │
                  │  • Lead qualification status  │                   │  • Branch / location details  │
                  └───────────────────────────────┘                   └───────────────────────────────┘
```

### 4.2 Routing Comparison: Inbound vs. Outbound

| Attribute | Path A: Inbound Calls | Path B: Outbound Calls |
| --- | --- | --- |
| **Who starts the call** | Customer | System, from approved call list |
| **AI involvement** | **None.** The AI is bypassed completely | Outbound AI voice agent handles the conversation |
| **Routing mechanism** | Static carrier-level forwarding | SIP trunk with configured outbound caller ID |
| **Destination** | Chloride Exide human support team | Customer / lead |
| **Escalation** | N/A (already handled by people) | Warm live transfer to designated staff line |
| **CRM write-back** | Handled by Chloride Exide's existing process | Automatic: transcript, summary, disposition tags |
| **SMS follow-up** | None | Automatic, triggered by call outcome |
| **Volume** | Unchanged from current operations | About 20 calls per working day |

### 4.3 Outbound Call Lifecycle

```
 [1] TRIGGER        [2] CONVERSATION        [3] RESOLUTION          [4] POST-CALL
 ─────────────      ──────────────────      ──────────────────      ─────────────────────
 CRM / list    ──►  Greeting & identity ──► • Tier-1 guidance  ──►  • CRM write-back
 record pulled      confirmation            • Booking made          • SMS dispatched
 with context       Purpose of call         • Warm transfer         • Disposition tagged
                    Triage questioning      • Callback noted
                                            • Polite close
```

| Stage | System Action | Data Flow |
| --- | --- | --- |
| **1. Trigger** | Pull next approved contact during the calling window, within the daily pacing limit | CRM → Agent (name, product history, lead source, call purpose) |
| **2. Conversation** | Run the scripted conversation flow and Tier-1 triage logic against the approved knowledge base | Live audio ↔ speech recognition / synthesis |
| **3. Resolution** | Give Tier-1 guidance, book on calendar, transfer to a person, or close | Agent → Calendar API / Transfer line |
| **4. Post-Call** | Write the full record to CRM and send the outcome-specific SMS | Agent → CRM API; Agent → SMS Gateway |

### 4.4 Integration Components

| Component | Function | Integration Method |
| --- | --- | --- |
| **Telephony** | Outbound dialing with configured caller ID; static forwarding of inbound numbers to human support | SIP trunk / carrier configuration |
| **CRM & Customer Database** | Source of call lists and context; system of record for transcripts, summaries and dispositions | REST API and/or webhooks |
| **SMS Gateway** | Post-call SMS based on call outcome | Chloride Exide's SMS provider API |
| **Calendar** | Availability lookup and direct booking for technician visits and sales consultations | Calendar API |
| **Knowledge Base** | Approved Tier-1 troubleshooting and Dial-a-Battery qualification content | Ingested and version-controlled at build |
| **Voice Model** | Production voice (authorized clone or approved stock voice) | AI speech synthesis provider |

### 4.5 Escalation Logic

The agent transfers the call to a person when **any** of the following applies:

- The customer asks to speak with a person.
- The question falls outside the approved Tier-1 knowledge base.
- The customer reports a safety concern (e.g. a swollen, leaking or overheating battery, burning smell, or electrical hazard).
- The customer raises a complaint, warranty dispute or pricing exception.
- The agent cannot reach a confident Tier-1 outcome after the defined number of clarification attempts.

If no transfer line is available (e.g. outside staffed hours), the agent records a **callback request**, tags the CRM record and sends a confirmation SMS.

---

## 5. 30-Day Phased Implementation Schedule

### 5.1 Phase Overview

```
 Day:  1    5 6          15 16        23 24        30
       ├────┤ ├───────────┤ ├──────────┤ ├──────────┤
       │ P1 │ │    P2     │ │    P3    │ │    P4    │
       └────┘ └───────────┘ └──────────┘ └──────────┘
       Discovery  Outbound     Integration  Deployment &
       & Telephony Build &     & Pipeline   Production
       Setup      Prompting    Testing      Launch
                                          ▲            ▲
                                       UAT Sign-off  Go-Live &
                                                     Month 1 Decision Gate
```

### 5.2 Detailed Phase Breakdown

| Phase | Days | Key Activities | Deliverables | Chloride Exide Inputs Required |
| --- | --- | --- | --- | --- |
| **P1: Discovery & Telephony Setup** | 1–5 | • Kickoff workshop with Dominic and team<br>• Map Tier-1 battery, Dial-a-Battery and solar/inverter decision logic<br>• Define CRM destination fields for transcript, summary and disposition tags<br>• Confirm SMS provider credentials and message templates<br>• Confirm inbound forwarding targets and outbound caller ID<br>• Define escalation lines, calling windows and pacing rules | • Signed-off discovery document<br>• Disposition tag taxonomy<br>• Integration field map<br>• Telephony configuration plan | Knowledge base documents, CRM/SMS/calendar access, forwarding numbers, transfer line(s), voice consent and reference audio |
| **P2: Outbound Build & Prompting** | 6–15 | • Ingest and structure approved troubleshooting documentation<br>• Build outbound conversation flows (follow-up, battery triage, Dial-a-Battery qualification, solar/inverter triage)<br>• Configure warm transfer and calendar booking logic<br>• Build SMS trigger logic per disposition<br>• Calibrate production voice (clone, or stock voice pending consent) | • Working outbound agent in staging<br>• Conversation flow documentation<br>• SMS template set<br>• Voice sample for approval | Review of conversation flows and SMS templates; voice approval |
| **P3: Integration & Pipeline Testing** | 16–23 | • End-to-end testing of CRM write-back accuracy<br>• SMS delivery testing for every trigger<br>• Warm live transfer testing (both triggers)<br>• Calendar booking validation<br>• Inbound forwarding verification (confirming the AI is bypassed)<br>• User Acceptance Testing (UAT) with Chloride Exide staff | • UAT test log<br>• Defect resolution log<br>• **UAT sign-off** | UAT participants (1–2 staff); sign-off |
| **P4: Deployment & Production Launch** | 24–30 | • Launch live outbound calling in controlled batches, ramping to ~20 calls/day<br>• Live monitoring of transfers, bookings and CRM sync<br>• Same-day fixes to prompts and logic (Month 1 optimization begins)<br>• Handover session and documentation | • Live production system<br>• Launch-week performance summary<br>• Handover pack<br>• **Month 1 review & decision gate** | Confirmation of production call lists; staff availability for live transfers |

### 5.3 Launch-Week Ramp Plan

| Launch Day | Daily Call Volume | Focus |
| --- | --- | --- |
| Day 24 | ~5 calls | Controlled pilot, with every call reviewed |
| Day 25–26 | ~10 calls | Validate transfers, bookings and SMS in production |
| Day 27–28 | ~15 calls | Check stability and CRM data quality |
| Day 29–30 | ~20 calls | Target steady-state pacing |

### 5.4 Schedule Dependencies

The 30-day schedule starts when **both** the signed proposal and the $500 trial deposit are received. It assumes:

- Knowledge base documentation, CRM/SMS/calendar access and telephony details are provided by **Day 5**.
- Review feedback on conversation flows is returned within **2 working days**.
- UAT participants are available during **Days 16–23**.

Delays in client inputs move the schedule by the same amount.

---

## 6. 3-Month Engagement Roadmap & Retainer Phasing

### 6.1 Roadmap Overview

```
 ┌──────────────────────┬──────────────────────┬──────────────────────┬──────────────────────────┐
 │       MONTH 1        │       MONTH 2        │       MONTH 3        │       MONTH 4+           │
 │   Days 1–30          │   Days 31–60         │   Days 61–90         │   Ongoing                │
 ├──────────────────────┼──────────────────────┼──────────────────────┼──────────────────────────┤
 │ Build, Launch &      │ Performance          │ Stabilization &      │ Run-State                │
 │ Initial Optimization │ Optimization         │ Run-State Transition │ Maintenance              │
 ├──────────────────────┼──────────────────────┼──────────────────────┼──────────────────────────┤
 │ Funded by:           │ Funded by:           │ Included in          │ Funded by:               │
 │ $500 Trial Deposit   │ $3,500 Milestone 2   │ $4,000 setup         │ $100/month Retainer      │
 └──────────┬───────────┴──────────────────────┴──────────────────────┴──────────────────────────┘
            │
            ▼
   ◆ DECISION GATE (Day 30): Chloride Exide elects to proceed → $3,500 due before Month 2 begins
```

### 6.2 Month-by-Month Detail

| Period | Objective | Key Activities | Outputs |
| --- | --- | --- | --- |
| **Month 1** (Days 1–30) | Build, launch and validate | 30-day implementation (Section 5); launch-week live tuning; initial optimization of prompts, triage paths and transfer thresholds | Live system; launch-week performance summary; **Month 1 review** |
| **◆ Decision Gate** (Day 30) | Go / no-go | Joint review of call outcomes, CRM data quality, transfer and booking rates, and customer feedback | Chloride Exide's written election to proceed |
| **Month 2** (Days 31–60) | Improve performance | Tune conversation flows from real transcripts; improve Tier-1 troubleshooting accuracy; refine Dial-a-Battery qualification; adjust SMS content and triggers; reduce unnecessary transfers | **Month 2 optimization report** with before/after metrics |
| **Month 3** (Days 61–90) | Stabilize and hand over to run-state | Confirm CRM data integrity end-to-end; finalize disposition taxonomy; document the run-state operating procedure; confirm the maintenance and change-request process | **Run-state readiness review**; final handover |
| **Month 4+** | Reliable ongoing operation | Maintenance retainer begins (Section 6.4) | Monthly health check |

### 6.3 Performance Metrics Tracked

| Metric | Definition | Why It Matters |
| --- | --- | --- |
| **Connect Rate** | Answered calls ÷ calls attempted | List quality and calling-window effectiveness |
| **Tier-1 Resolution Rate** | Calls resolved by approved guidance without transfer | Load taken off human support |
| **Booking Rate** | Calendar bookings ÷ connected calls | Conversion to technician or sales activity |
| **Dial-a-Battery Qualification Rate** | Qualified Dial-a-Battery leads ÷ relevant connected calls | Direct revenue pipeline |
| **Warm Transfer Rate & Success** | Transfers started, and the share that connect | Escalation health and staff coverage |
| **CRM Sync Integrity** | Completed calls with a full, correctly mapped CRM record | Data reliability (target: 100%) |
| **SMS Delivery Rate** | SMS delivered ÷ SMS triggered | Follow-up reliability |

### 6.4 Maintenance Retainer: $100/month (from Month 4)

| Included in Retainer | Not Included (Change Request) |
| --- | --- |
| System uptime and webhook health monitoring | New conversation flows, campaigns or use cases |
| API and carrier connection maintenance | Inbound AI agent of any kind |
| Routine bug fixes and error resolution | Email automation or campaigns |
| Minor prompt updates for changed product specs or troubleshooting steps | New system integrations or CRM migration |
| Disposition tag and SMS template text adjustments | Material increases in call volume or new dialing campaigns |
| Monthly health check summary | Third-party usage fees |

---

## 7. Commercial Investment Schedule & Third-Party Cost Model

### 7.1 Setup Investment Schedule

| Milestone | Trigger / Due Date | Covers | USD | KES (@130) |
| --- | --- | --- | --- | --- |
| **1. Trial Deposit** | Due **at signing** | Full 30-day build (Phases P1–P4), production launch and Month 1 optimization | **$500** | **KSh 65,000** |
| **2. Setup Balance** | Due **before Month 2 optimization begins**, when Chloride Exide elects to proceed at the Day 30 decision gate | Month 2 optimization, Month 3 stabilization and run-state transition | **$3,500** | **KSh 455,000** |
| **Total One-Time Setup Investment** | | | **$4,000** | **KSh 520,000** |

### 7.2 Recurring Fees

| Fee | Start | USD | KES (@130) |
| --- | --- | --- | --- |
| **Maintenance Retainer** | First month after the 3-month onboarding period (Month 4) | **$100 / month** | **KSh 13,000 / month** |

### 7.3 Total Cost of Engagement (Professional Fees Only)

| Period | Professional Fees (USD) | Cumulative (USD) | Cumulative (KES @130) |
| --- | --- | --- | --- |
| Month 1 | $500 | $500 | KSh 65,000 |
| Month 2 | $3,500 | $4,000 | KSh 520,000 |
| Month 3 | $0 | $4,000 | KSh 520,000 |
| Months 4–12 (9 × $100) | $900 | $4,900 | KSh 637,000 |
| **First-Year Total** | | **$4,900** | **KSh 637,000** |

*Excludes third-party usage costs (Section 7.4), which Chloride Exide pays directly.*

### 7.4 Third-Party Usage Cost Model

Chloride Exide pays all raw third-party infrastructure costs **directly to the providers**, through accounts held or connected in Chloride Exide's name. No markup is applied.

| Cost Category | What It Covers | Billing Basis | Paid By |
| --- | --- | --- | --- |
| **Telephony** | Outbound carrier minutes, SIP trunking, number provisioning, forwarded inbound minutes (where the carrier charges for them), live transfer leg minutes | Per minute / per number per month | Chloride Exide (direct) |
| **AI Speech Processing** | Speech-to-text (transcription) and text-to-speech (voice synthesis) minutes, plus language model processing for the conversation | Per minute / per usage unit | Chloride Exide (direct) |
| **SMS** | Post-call SMS carrier fees | Per message segment | Chloride Exide (direct) |

#### Illustrative Monthly Volume Model

The table below shows expected **usage volumes** at target pacing so Chloride Exide can budget against its own negotiated provider rates. Actual rates are confirmed during Discovery (Phase P1).

| Assumption | Value | Basis |
| --- | --- | --- |
| Working days per month | ~22 | Monday–Friday |
| Outbound call attempts per day | ~20 | Target pacing |
| **Outbound call attempts per month** | **~440** | 20 × 22 |
| Connect rate (planning assumption) | ~60% | Validated in Month 1 |
| **Connected conversations per month** | **~264** | 440 × 60% |
| Average connected call duration | ~4 minutes | Includes triage and booking |
| **AI-handled talk minutes per month** | **~1,056 minutes** | 264 × 4 |
| Post-call SMS per month | ~264 | ~1 SMS per connected call |

**Monthly usage estimate formula:**

```
 Monthly Usage Cost ≈ (AI talk minutes × telephony rate per minute)
                    + (AI talk minutes × AI speech/model rate per minute)
                    + (Transfer leg minutes × telephony rate per minute)
                    + (SMS sent × SMS rate per message)
                    + (Number rental per month)
```

A provider-specific cost estimate, using actual rates for Chloride Exide's chosen telephony and SMS providers, will be delivered at the end of Phase P1, before production traffic starts.

### 7.5 Commercial Terms

- **Contract currency:** USD. KES amounts are shown at the reference rate of 130 KES/USD for convenience. Invoices may be settled in KES at the agreed equivalent.
- **Schedule start:** The 30-day implementation begins when the signed proposal and the $500 trial deposit have both been received.
- **Decision gate:** At the end of Month 1, Chloride Exide decides in writing whether to proceed. If it does not proceed, the engagement ends at the close of Month 1 and **no further setup fees are due**.
- **Milestone 2:** The $3,500 balance must be received before Month 2 optimization work begins.
- **Retainer:** Billed monthly in advance from Month 4.
- **Usage costs:** Paid directly by Chloride Exide to third-party providers and not included in any professional fee above.
- **Scope changes:** Any item listed under Section 3.2 (Exclusions) needs a written change request with separately agreed scope and pricing.

---

## 8. Technical Prerequisites & Sign-Off Checklist

### 8.1 Technical Prerequisites (Required by Day 5)

| # | Prerequisite | Description | Owner | Status |
| --- | --- | --- | --- | --- |
| 1 | **Inbound Forwarding Target** | Direct number(s) for Chloride Exide's human support team where all inbound calls will be forwarded | Chloride Exide | ☐ |
| 2 | **Outbound Caller ID & Numbers** | Approved outbound caller ID and number(s); confirmation of carrier / SIP provider | Chloride Exide | ☐ |
| 3 | **Warm Transfer Line(s)** | Staff line(s) for live transfers, with staffed hours | Chloride Exide | ☐ |
| 4 | **CRM Access & Field Mapping** | API/webhook access; confirmed fields for **full transcript**, **summary text** and **disposition tag** | Chloride Exide | ☐ |
| 5 | **Call List Source** | Approved lead and customer lists (or CRM views) for outbound calling, with confirmed contact consent | Chloride Exide | ☐ |
| 6 | **Troubleshooting Source Materials** | Approved guides for automotive batteries, **Dial-a-Battery qualification**, solar panels, inverters and energy storage | Chloride Exide | ☐ |
| 7 | **SMS Gateway Credentials** | API access for the preferred SMS provider; approved sender ID | Chloride Exide | ☐ |
| 8 | **Calendar Access** | Access to technician and sales consultation calendars; booking rules (slot length, regions, lead time) | Chloride Exide | ☐ |
| 9 | **Voice Clone Consent & Audio** | **Explicit written consent** from the voice owner and **clean reference audio** (quiet room, no background noise or music) | Chloride Exide | ☐ |
| 10 | **Third-Party Provider Accounts** | Telephony, AI speech and SMS accounts held or connected in Chloride Exide's name, with billing set up | Chloride Exide | ☐ |
| 11 | **Compliance Confirmation** | Confirmation that outbound calling, call recording/transcription disclosure and SMS messaging follow Chloride Exide's data protection obligations (including the Kenya Data Protection Act, 2019) and internal policies | Chloride Exide | ☐ |
| 12 | **Project Point of Contact** | A named decision-maker and a technical contact for integrations and UAT | Chloride Exide | ☐ |

### 8.2 Scope Acknowledgement Checklist

By signing, Chloride Exide confirms its understanding of the following scope boundaries:

| # | Acknowledgement | Initial |
| --- | --- | --- |
| A1 | **Inbound AI is out of scope.** All inbound calls bypass the AI completely and are statically forwarded to Chloride Exide's human support team. | ____ |
| A2 | The AI agent is **outbound only**, paced at about **20 calls per working day**. | ____ |
| A3 | Technical guidance is **Tier-1 only**, based solely on Chloride Exide–approved documentation. Anything beyond Tier-1, or any customer request for a person, is warm-transferred to staff. | ____ |
| A4 | There is **no dynamic cross-call or in-session memory**. Context comes from the call trigger, and results are written to the CRM after each call. | ____ |
| A5 | Automated follow-up is **SMS only**. Email sequencing and campaigns are excluded. | ____ |
| A6 | The production voice clone needs **explicit written consent** and **clean reference audio** supplied by Chloride Exide. | ____ |
| A7 | **Third-party usage costs** (telephony, AI speech processing, SMS) are paid directly by Chloride Exide. | ____ |

### 8.3 Commercial Sign-Off

| Item | Amount | Due | Confirmed |
| --- | --- | --- | --- |
| Trial Deposit | $500 USD (KSh 65,000) | At signing | ☐ |
| Setup Balance (Milestone 2) | $3,500 USD (KSh 455,000) | Before Month 2 optimization, on election to proceed | ☐ |
| **Total Setup Investment** | **$4,000 USD (KSh 520,000)** | | |
| Maintenance Retainer | $100 USD / month (KSh 13,000) | Monthly from Month 4 | ☐ |

### 8.4 Immediate Next Steps

1. **Review and approve** this proposal, including the scope acknowledgements in Section 8.2.
2. **Sign** the authorization block below.
3. **Remit the $500 trial deposit** (KSh 65,000) to secure Day 1 of the implementation schedule.
4. **Nominate** a project decision-maker and technical contact.
5. **Schedule the kickoff workshop** (Day 1) and begin handing over the Section 8.1 prerequisites.

### 8.5 Authorization

| | **Chloride Exide** | **Service Provider** |
| --- | --- | --- |
| **Name** | | Kamunya Maina |
| **Title** | | |
| **Signature** | | |
| **Date** | | |

---

*This proposal is confidential and intended solely for Chloride Exide. Pricing is valid for 30 days from the date of issue.*
