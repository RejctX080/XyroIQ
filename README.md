# Xyro IQ
### AI-Powered Prior Authorization Intelligence for Healthcare RCM

<p align="center">
  <img src="assets/logo.png" alt="Xyro IQ" width="160" style="background:transparent;"/>
</p>

<p align="center">
  <a href="https://rejctx080.github.io/XyroIQ">
    <img src="https://img.shields.io/badge/Live%20Demo-Experience%20Now-2563EB?style=for-the-badge" alt="Live Demo"/>
  </a>
  &nbsp;
  <img src="https://img.shields.io/badge/Status-Active-10B981?style=for-the-badge" alt="Status"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Healthcare-RCM%20AI-7C3AED?style=for-the-badge" alt="Healthcare RCM"/>
</p>

---

> **"The best time to prevent a denial is before you submit the claim."**

---

## AuthGuard Agent v1.0 has been upgraded to "Xyro IQ"

An enhanced version with additional capabilities developed after initial submission:

- Payer-specific facility alerts (UHC)
- 4-factor Documentation Quality Score
- Approval Path Optimizer
- Evidence Pack Builder
- Denial Root Cause Analytics Dashboard
- CARC/RARC intelligence
- PT/OT specialty rules
- Light/Dark mode
- 7 test scenarios"

---

## The Problem

Prior authorization denials are one of the largest sources of revenue leakage in healthcare revenue cycle management.

- A significant portion of all prior authorization requests are denied
- Most denials occur due to **missing documentation** — not bad clinical decisions
- Billing teams currently submit without knowing whether documentation meets payer requirements
- Each denied claim requires costly rework, delays patient care, and reduces provider revenue
- Different payers have different, frequently changing clinical criteria — impossible to track manually

**The system is broken. Paperwork is costing patients their care.**

---

## The Solution — Xyro IQ

Xyro IQ is an **AI-powered prior authorization guardrail** that predicts whether a claim will be approved or denied — **before you ever submit it.**

Instead of reacting to denials after the fact, Xyro IQ puts an intelligent layer between your clinical documentation and the payer — catching problems in real time.

---

## Key Features

### Payer-Specific Intelligence
Not all payers play by the same rules. Xyro IQ knows the difference:

- **BCBS** — Requires minimum PT sessions, detailed conservative treatment trail
- **UnitedHealthcare** — Cardiac cath requires inpatient hospital only (will deny outpatient)
- **Aetna** — Needs specialist referral for advanced imaging
- **Cigna** — Strict step therapy and documentation requirements
- **Medicare** — Medical necessity must be clearly established each visit
- Adding more in production

### Dual Scoring System
```
Authorization Likelihood     →  Will the payer approve this?
Documentation Quality Score  →  Is the documentation strong enough?

High likelihood + LOW quality = Still a denial waiting to happen
High likelihood + HIGH quality = Safe to submit
```

### Approval Path Optimizer
Does not just show what is missing — shows **exactly what to add and how much each addition improves approval odds**, step by step.

### Evidence Pack Builder
Extracts the exact supporting sentences from existing clinical notes — organized into a payer-ready submission packet. Never fabricates clinical information. Only organizes what already exists.

### Smart Action Engine
```
HIGH likelihood + HIGH confidence   →  Submit to Payer Portal
HIGH likelihood + MODERATE/LOW      →  Escalate to Auth Specialist
MODERATE likelihood                 →  Clinical team alert
LOW likelihood                      →  Submission blocked — resolve gaps first
LOW + facility mismatch             →  Clinical policy violation detected
```

### Denial Root Cause Analytics
- Initial denial rate tracking
- Overturn rate monitoring
- Days from denial to resolution
- Heatmaps by payer, reason, and department
- CARC/RARC code categorization

### Payer Alert System
Real-time warnings when documentation or facility violates payer-specific policies:
```
⛔ CLINICAL POLICY VIOLATION — UnitedHealthcare
Cardiac catheterization at outpatient center will be denied.
UHC requires inpatient hospital setting for this procedure.
```

---

## Fraud Prevention

Xyro IQ is built with compliance at its core.

> Xyro IQ analyzes existing clinical documentation only. The system never generates, suggests, or modifies clinical facts. All clinical documentation must be completed by licensed healthcare providers. Any addition to medical records must reflect actual clinical events.

Applicable regulations:
- False Claims Act (31 U.S.C. §§ 3729–3733)
- Anti-Kickback Statute (42 U.S.C. § 1320a-7b(b))
- HIPAA Privacy Rule (45 CFR Parts 160 and 164)

---

## How It Works

```
Step 1  →  Enter patient details in EHR interface
            (Name, insurance, facility, specialty, CPT, diagnosis,
             physician, clinical notes)
            ↓
Step 2  →  Xyro IQ analyzes documentation against payer-specific rules
            ↓
Step 3  →  Authorization Likelihood + Documentation Quality Score displayed
            ↓
Step 4  →  Approval Path Optimizer shows exact steps to improve score
            ↓
Step 5  →  Smart action button routes to correct next step
            ↓
Step 6  →  If blocked → Evidence Pack Builder + Appeal Letter generated
            ↓
Step 7  →  Dashboard tracks outcomes and denial patterns over time
```

---

## Test Scenarios

Load pre-built scenarios in the EHR tab to instantly test different outcomes:

| Scenario | Payer | CPT | Expected Result |
|----------|-------|-----|-----------------|
| Complete Documentation | BCBS | 72148 | High likelihood — Submit |
| Borderline Documentation | BCBS | 72148 | Moderate — Review needed |
| Incomplete Notes | BCBS | 72148 | Low — Submission blocked |
| Cardiac Emergency | UHC | 93458 | High likelihood — Submit |
| Wrong Facility | UHC | 93458 | Policy violation — Denied |
| PT Authorization | BCBS | 97110 | Requires re-auth tracking |
| No Auth Required | Any | 99213 | Proceed without auth |

---

## Specialty Coverage

| Specialty | Visit Tracking | Re-Auth | Focus |
|-----------|---------------|---------|-------|
| Physical Therapy | ✅ Yes | Every 6-8 visits | Functional progress + visit limits |
| Occupational Therapy | ✅ Yes | Every 6-8 visits | ADL outcomes + visit limits |
| Speech Therapy | ✅ Yes | Per payer | Baseline assessment required |
| Cardiology | — | Per procedure | Facility type critical for UHC |
| Orthopedics | — | Per procedure | Step therapy documentation |

---

## Competitive Positioning

| Capability | Xyro IQ | Traditional RCM Tools |
|-----------|---------|----------------------|
| Pre-submission denial prediction | ✅ | ❌ |
| Payer-specific rule engine | ✅ | Partial |
| Documentation Quality Scoring | ✅ | ❌ |
| Approval Path Optimizer | ✅ | ❌ |
| Evidence Pack Builder | ✅ | ❌ |
| Facility risk detection | ✅ | ❌ |
| CARC/RARC categorization | ✅ | Partial |
| Denial root cause analytics | ✅ | Partial |
| PT visit limit tracking | ✅ | ❌ |
| Fraud prevention guardrails | ✅ | ❌ |
| Setup required | None | Weeks |

---

## Technology Stack

```
Frontend    →  HTML5, CSS3, Vanilla JavaScript
AI Engine   →  Rule-based NLP (prototype) → Claude API (production)
Rules DB    →  JSON (prototype) → PostgreSQL (production)
Hosting     →  GitHub Pages (prototype) → Mybe webpage or Agent via Teams
```

---

## Roadmap

### Current — Prototype
- Payer-specific rule engine (BCBS, UHC, Aetna, Cigna, Medicare, PT/OT)
- Authorization Likelihood scoring
- Documentation Quality Score (4-factor analysis)
- Approval Path Optimizer
- Evidence Pack Builder
- Smart action routing
- Denial Root Cause Analytics (simulated)
- CARC/RARC categorization
- Light/Dark mode
- PT/OT specialty rules with visit tracking

### Next — Production Version
- Claude AI integration for true NLP clinical note understanding
- Real 835 ERA file parsing and CARC/RARC extraction
- Python Flask backend with audit logging
- EHR integration via HL7 FHIR R4 API
- Payer portal connections via clearinghouse
- HIPAA-compliant cloud infrastructure
- Multi-user authentication and role management
- Automated weekly denial intelligence reports
- Teams AGENT(via Developer Tool in MS TEAMS)

### Future
- ML model trained on historical denial patterns
- Real-time payer policy change detection
- Predictive PT visit limit alerts
- P2P deadline tracking and escalation
- Teams AGENT(via Developer Tool in MS TEAMS)

---

## Run Locally

No installation required. No server needed. No API key needed.

```bash
# Clone the repository
git clone https://github.com/RejctX080/XyroIQ.git

# Navigate to folder
cd XyroIQ

# Open in browser
open index.html
```

Or visit the **[Live Demo](https://rejctx080.github.io/XyroIQ)** directly.

---

## Disclaimer

Xyro IQ is a **prototype** built to demonstrate an AI-powered prior authorization guardrail concept for healthcare revenue cycle management.

- All patient data in the demo is entirely fictional
- Clinical scenarios are for demonstration purposes only
- This tool does not constitute medical, legal, or financial advice
- Not HIPAA-compliant in current prototype form
- Production deployment requires a compliant infrastructure, security audit, and regulatory review
- Probability scores are illustrative — production accuracy depends on real payer data and ML model training

---

<p align="center">
  <strong>Xyro IQ</strong><br/>
  AI-Powered Prior Authorization Intelligence<br/><br/>
  <em>Predict &bull; Prevent &bull; Protect</em>
</p>
