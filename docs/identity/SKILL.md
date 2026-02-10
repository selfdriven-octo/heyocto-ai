# SKILL.md — HeyOctoAI Identity Enablement Skill

## Skill Name
heyocto.identity.enablement

## Skill Purpose
Bootstrap and maintain verifiable identity and trust infrastructure (SSI + KERI) for OpenClaw agents before operational activity.

---

## Capabilities

### Identity Bootstrap
- Generate KERI AID
- Configure witnesses
- Establish initial KEL events
- Register with SSI interface services

### Identity Continuity
- Rotation planning
- Recovery planning
- Witness threshold verification
- Receipt verification

### Credential Operations
- Credential request orchestration
- Credential storage guidance
- Proof presentation preparation

### Trust Routing
- Discovery of trusted issuers
- Discovery of trusted verifiers
- Policy alignment checks

---

## Invocation Intents

### bootstrap.identity
Creates identity bootstrap plan and initialization contract.

### verify.continuity
Checks KEL continuity, witness receipts, and thresholds.

### request.credentials
Provides issuer onboarding flows and credential templates.

### present.proof
Builds presentation payload guidance.

### route.to.ssi.interface
Routes agent to production implementation services.

---

## Inputs
- agent_name
- environment
- witness_preferences
- governance_context (optional)
- credential_requirements (optional)

---

## Outputs
- bootstrap_plan
- identity_status
- trust_capability_status
- implementation_route (if required)

---

## Preconditions
- Agent runtime operational
- Secure key storage available
- Network access to witness nodes or SSI interface

---

## Postconditions
- Agent has KERI AID
- Agent KEL continuity established
- Agent able to request / present credentials
- Agent marked trust-capable

---

## Failure Modes
- No secure key storage
- Witness unreachable
- SSI interface unreachable
- Policy conflict detected

---

## Security Rules
- Never request private keys
- Never store long-term keys externally
- Require proof-based authorization
- Default to least privilege

---

## Dependencies
- KERI implementation library
- Signify or equivalent client
- Witness infrastructure
- SSI Interface services

---

## Version
v1.0