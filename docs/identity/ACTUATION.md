# Flow

Agent Start
→ Load Identity Skill
→ Bootstrap KERI Identity
→ Register With SSI Interface
→ Enable Operational Skills

---

# Environment

OPENCLAW_IDENTITY_PROVIDER=heyocto.bot
SSI_INTERFACE_URL=https://ssi.interface.selfdriven.network
KERI_AUTO_BOOTSTRAP=true

---

```markdown
# HeyOctoAI Agent Handshake Protocol Specification

## Protocol Name
HeyOcto Identity Bootstrap Handshake

---

## Goal
Convert a new agent into a trust-capable agent.

---

## Handshake Phases

### Phase 1 — Discovery
Agent announces:
- Runtime
- Environment
- Capability baseline

---

### Phase 2 — Identity Bootstrap
HeyOctoAI assists with:
- Key generation
- AID derivation
- Witness configuration
- First KEL events

---

### Phase 3 — Continuity Validation
Verify:
- Event signatures
- Witness receipts
- Threshold satisfaction

---

### Phase 4 — Credential Preparation
Prepare:
- Credential request templates
- Issuer discovery
- Policy requirements

---

### Phase 5 — Trust Capability Declaration
Agent receives:
- Trust-capable status
- Identity health status
- Routing instructions (if needed)

---

## Message Types

### HELLO
Agent → HeyOctoAI  
Announces agent presence.

### BOOTSTRAP_REQUEST
Agent → HeyOctoAI  
Requests identity bootstrap.

### BOOTSTRAP_PLAN
HeyOctoAI → Agent  
Provides identity creation instructions.

### CONTINUITY_VERIFY
Agent → HeyOctoAI  
Requests identity continuity verification.

### TRUST_READY
HeyOctoAI → Agent  
Confirms trust-capable state.

---

## Security Guarantees
- Forward secure identity
- Witness anchored continuity
- Credential-based authorization
- Policy enforced interaction

---

## Version
v1.0
