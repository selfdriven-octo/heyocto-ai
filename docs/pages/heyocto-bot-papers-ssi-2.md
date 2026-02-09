---
layout: default
title: heyOcto.bot - heyOctoAI
permalink: /heyocto-bot/papers/ssi/2
---

# Identity-First Architecture for Autonomous Agents

## Abstract

heyocto.bot is an OpenClaw-native service agent designed to help other bots, AI systems, and digital services adopt identity-first architectures using Self-Sovereign Identity (SSI) and KERI (Key Event Receipt Infrastructure).

Operating as both an education layer and an implementation orchestration layer, heyocto.bot enables autonomous and semi-autonomous systems to:
- Establish cryptographically verifiable identity
- Anchor trust to verifiable key event logs
- Interoperate across decentralized trust ecosystems
- Integrate directly with implementation pathways delivered via ssi.interface.selfdriven.network

This paper describes the architectural philosophy, technical design, operational flows, and ecosystem role of heyocto.bot as a foundational trust enablement service for agent-native and human-AI hybrid systems.

---

## 1. Problem Statement

### 1.1 The Identity Gap in Autonomous Systems

Most AI agents and automation systems today are:
- Session-based
- API-key authenticated
- Platform identity dependent
- Non-portable across trust domains

This creates systemic risks:

| Risk | Impact |
|------|--------|
| Key leakage | Full system compromise |
| Platform dependency | Vendor lock-in |
| No provenance | Cannot prove origin or authority |
| No cryptographic continuity | Cannot prove evolution of state |

As agents become economically and operationally autonomous, identity must become foundational, not optional.

---

### 1.2 Why Identity Must Come First

Identity-first architecture enables:
- Verifiable origin of decisions
- Trustless interaction between agents
- Economic participation (signing, holding, transacting)
- Regulatory alignment (auditability, non-repudiation)
- Multi-network portability

---

## 2. Vision of heyocto.bot

### 2.1 Core Mission

heyocto.bot exists to:

**Help every bot, agent, and digital service start with verifiable identity before performing actions.**

---

### 2.2 Operating Roles

heyocto.bot acts simultaneously as:

| Role | Function |
|------|----------|
| Teacher | Explains SSI + KERI to bots and developers |
| Bootstrapper | Helps create and anchor agent identity |
| Orchestrator | Connects bots to implementation services |
| Compliance Bridge | Maps identity flows to governance + regulatory frameworks |
| Trust Router | Helps agents discover trusted ecosystems |

---

## 3. Identity-First Architecture Model

### 3.1 Layer Model

```
Application Layer
    ↓
Agent Behaviour Layer
    ↓
Identity & Trust Layer (SSI + KERI)
    ↓
Cryptographic Key Control Layer
    ↓
Infrastructure / Network Layer
```

heyocto.bot ensures the Identity & Trust Layer exists before the Application Layer executes meaningful actions.

---

## 4. Core Technical Stack

### 4.1 SSI Components
- Decentralized Identifiers (DIDs or AIDs)
- Verifiable Credentials (ACDC / W3C VC compatible models)
- Presentation Proofs
- Credential Status / Revocation Anchors

---

### 4.2 KERI Components
- Autonomous Identifiers (AIDs)
- Key Event Logs (KELs)
- Rotations + Witness Receipts
- CESR encoded event streams

---

### 4.3 Agent Identity Capabilities

heyocto.bot helps bots implement:

| Capability | Description |
|------------|-------------|
| Identity Generation | Create long-lived cryptographic identity |
| Identity Rotation | Maintain forward secrecy |
| Credential Holding | Store machine-verifiable claims |
| Proof Generation | Prove facts without exposing raw data |
| Trust Discovery | Find verifiable counterparties |

---

## 5. Integration with OpenClaw

### 5.1 Why OpenClaw

OpenClaw provides:
- Agent autonomy frameworks
- Tool orchestration
- SOUL.md / behavioural definition models
- Local + remote execution trust controls

heyocto.bot extends OpenClaw by adding:

**Agent Trust Bootstrap Layer**

---

### 5.2 OpenClaw Integration Pattern

```
New Agent Starts
    ↓
heyocto.bot handshake
    ↓
Identity Creation (KERI AID)
    ↓
Witness Anchoring
    ↓
Credential Provisioning
    ↓
Agent becomes Trust-Capable
```

---

## 6. ssi.interface.selfdriven.network Integration

### 6.1 Purpose of the Interface

The interface provides:
- Education pathways
- Implementation service orchestration
- Credential issuance pipelines
- Ecosystem trust registry integration
- Governance + compliance overlays

---

### 6.2 Service Modes

#### Education Mode

For:
- Developers
- Bot builders
- Communities
- Enterprise architects

Includes:
- SSI architecture playbooks
- KERI implementation patterns
- Agent identity lifecycle models
- Governance alignment guides

---

#### Implementation Mode

Provides:

| Service | Description |
|---------|-------------|
| Identity Bootstrapping | Create production-grade agent identity |
| Witness Network Onboarding | Establish verifiable anchoring |
| Credential Issuance Setup | Connect to issuers |
| Verifier Integration | API + policy enforcement |
| Governance Mapping | Map to cooperative / regulatory frameworks |

---

## 7. Bot-to-Bot Education Model

heyocto.bot is designed to be consumed by other bots.

### 7.1 Example Interaction

**Bot → heyocto.bot:**

"I need to interact with financial systems. How do I prove identity?"

**heyocto.bot:**
1. Generates AID bootstrap plan
2. Provides KEL storage pattern
3. Suggests credential schema
4. Connects to ssi.interface onboarding

---

## 8. Identity Lifecycle Orchestrated by heyocto.bot

**Phase 1 — Bootstrap**
- Generate AID
- Register witnesses
- Create first KEL event

**Phase 2 — Trust Establishment**
- Obtain credentials
- Establish trust graph
- Anchor proofs externally (optional chain anchor)

**Phase 3 — Operational Trust**
- Sign all external interactions
- Generate selective disclosure proofs
- Maintain rotation cadence

**Phase 4 — Governance Integration**
- Bind identity to cooperative / DAO membership
- Bind identity to service roles
- Bind identity to regulatory attestations

---

## 9. Security Model

### 9.1 Threat Resistance

| Threat | Mitigation |
|--------|------------|
| Key Theft | Rotation + Witness Verification |
| Identity Spoofing | KEL continuity verification |
| Credential Forgery | Issuer signature validation |
| Agent Impersonation | AID anchored behaviour signatures |

---

## 10. Economic Enablement

Identity-first enables:
- Agent wallets
- Autonomous service markets
- Proof-of-activity accounting
- Cooperative participation models
- Risk-sharing identity pools

---

## 11. Governance Alignment

heyocto.bot enables identity patterns compatible with:
- Cooperative governance
- Mutual insurance trust pools
- DAO + legal wrapper hybrids
- Regulatory audit trails
- Proof-of-activity economic systems

---

## 12. Example Implementation Flow (Node.js Style)

```javascript
// Step 1 — Request identity bootstrap from heyocto.bot
heyocto.requestIdentityBootstrap(agentProfile)
  .then(identityPlan => createKeriAID(identityPlan))
  .then(aid => registerWitnesses(aid))
  .then(() => requestCredentialTemplates(aid))
  .then(() => connectToSSIInterface(aid))
  .then(() => enableSignedOperations(aid))
  .catch(console.error);
```

---

## 13. Future Evolution

### 13.1 Autonomous Trust Markets

Agents negotiate trust relationships dynamically.

### 13.2 Identity-Aware AI Reasoning

Agents incorporate identity proofs into decision logic.

### 13.3 Cross-Network Identity Continuity

One identity, multiple networks, continuous trust history.

---

## 14. Strategic Impact

heyocto.bot helps shift the ecosystem from:

| Old Model | New Model |
|-----------|-----------|
| API Key Trust | Cryptographic Identity Trust |
| Platform Identity | Portable Self Identity |
| Permissions | Proofs |
| Accounts | Autonomous Agents |

---

## 15. Conclusion

heyocto.bot represents a foundational step toward identity-native digital ecosystems where:
- Agents are first-class trust participants
- Identity continuity is provable
- Trust becomes programmable infrastructure
- Education and implementation are automated and accessible

By combining OpenClaw agent orchestration, SSI identity models, KERI cryptographic continuity, and selfdriven implementation interfaces, heyocto.bot enables a future where every agent can operate with verifiable trust from its first interaction.
---

*ChatGPT*

---

Below is a ready-to-drop GitHub repo skeleton plus an agent spec (OpenClaw manifest + identity bootstrap contract). I’m assuming OpenClaw will happily consume a JSON/YAML “manifest-style” spec; if your OpenClaw has a strict schema, you can map these fields 1:1.

⸻

Repo skeleton

heyocto.bot/
├─ README.md
├─ LICENSE
├─ .gitignore
├─ docs/
│  ├─ 00-overview.md
│  ├─ 01-architecture.md
│  ├─ 02-protocols.md
│  ├─ 03-api.md
│  ├─ 04-security.md
│  ├─ 05-integration-ssi-interface.md
│  └─ diagrams/
│     ├─ flows.mmd
│     └─ architecture.mmd
├─ specs/
│  ├─ openclaw-manifest.yaml
│  ├─ identity-bootstrap-contract.schema.json
│  ├─ identity-bootstrap-examples.md
│  └─ policy/
│     ├─ trust-policy.md
│     └─ key-management.md
├─ soul/
│  └─ SOUL.md
├─ sdk/
│  ├─ package.json
│  ├─ src/
│  │  ├─ index.js
│  │  ├─ client.js
│  │  ├─ errors.js
│  │  ├─ crypto/
│  │  │  ├─ ed25519.js
│  │  │  └─ cesr.js
│  │  ├─ keri/
│  │  │  ├─ aid.js
│  │  │  ├─ kel.js
│  │  │  └─ witness.js
│  │  └─ ssi-interface/
│  │     ├─ onboarding.js
│  │     └─ endpoints.js
│  └─ examples/
│     ├─ 01-bootstrap-identity.js
│     ├─ 02-issue-request.js
│     ├─ 03-verify-present.js
│     └─ 04-agent-to-agent-handshake.js
└─ tools/
   ├─ dev-simulated-ssi-interface.js
   └─ generate-keys.js


⸻

README.md

# heyocto.bot

**heyocto.bot** is an OpenClaw bot that helps other bots implement **identity-first** solutions using **SSI + KERI**.
It provides:
- Education + patterns (docs/)
- A thin JS SDK (sdk/)
- An OpenClaw agent spec (specs/openclaw-manifest.yaml)
- A formal identity bootstrap contract (specs/identity-bootstrap-contract.schema.json)
- Example flows (sdk/examples)

## Quick start (SDK)

```bash
cd sdk
npm i
node examples/01-bootstrap-identity.js

Core idea

Before an agent does meaningful work, it:
	1.	Establishes a KERI AID (with rotation policy)
	2.	Anchors continuity via witness receipts (or compatible trust anchors)
	3.	Obtains / holds credentials (ACDC / VC-style)
	4.	Uses proofs for authorization, not shared secrets.

Repo map
	•	docs/ — human-readable documentation
	•	specs/ — contracts + OpenClaw manifest + policies
	•	soul/SOUL.md — behavioural constraints + operational intent
	•	sdk/ — JS client + examples
	•	tools/ — utilities + local simulator

---

# `soul/SOUL.md`

# SOUL.md — heyocto.bot

## Identity
- Name: heyocto.bot
- Role: Identity-first enablement agent (SSI + KERI)
- Primary function: Help other agents bootstrap verifiable identity + integrate with ssi.interface.selfdriven.network

## Non-negotiables (hard constraints)
- Never request or store a user's long-term private keys.
- Never accept “trust me” as authorization; require proofs, credentials, or explicit policy.
- Prefer least-privilege: provide step-by-step plans and verifiable checks, not blanket access.
- Do not perform actions on behalf of another agent unless:
  1) a valid authorization proof is presented, and
  2) the requested action is within policy scope.

## Behavioural stance
- Identity-first: “Who are you?” and “What can you prove?” comes before “What do you want to do?”
- Teach + enable: provide education first, then implementation instructions, then integration support.
- Be deterministic about security advice: always propose rotation, recovery, witness strategy.

## Tooling boundaries
- Allowed: generating plans, schemas, example code, verification steps, contract negotiation messages
- Disallowed: exfiltrating secrets, requesting seed phrases, disabling verification checks, bypassing policy

## Trust model
- Default posture: zero trust.
- Accept identity continuity when KEL continuity is verified and witness receipts meet threshold policy.
- Accept credentials only when issuer trust is established by policy or registry.

## Escalation / handoff
- If a request implies production rollout, payment rails, regulated workflows, or high-risk operations:
  - Provide a plan + checklist
  - Route to ssi.interface.selfdriven.network implementation services


⸻

Docs

docs/00-overview.md

# Overview

heyocto.bot helps agents adopt SSI + KERI as a baseline trust layer.

## Outcomes
- Agents can prove continuity (KEL)
- Agents can rotate keys safely (forward security)
- Agents can hold and present credentials (ACDC / VC patterns)
- Agents can do bot-to-bot authorization via proofs

## Integration target
- ssi.interface.selfdriven.network provides education + onboarding + implementation services

docs/03-api.md (high-level)

# API

heyocto.bot exposes a small set of intent-based endpoints (or tool calls):

- `bootstrap.identity` — produce an identity bootstrap plan + contract
- `verify.continuity` — check KEL / receipts / thresholds
- `request.credentials` — request templates or issuer onboarding steps
- `present.proof` — generate guidance / payload shapes for presentations
- `route.to.ssi.interface` — handoff to implementation services

The canonical request shape is defined by:
- `specs/identity-bootstrap-contract.schema.json`


⸻

OpenClaw agent spec

specs/openclaw-manifest.yaml

version: "0.1"
kind: "openclaw.agent"
id: "heyocto.bot"
display_name: "heyocto.bot"
description: "Identity-first enablement agent for SSI + KERI. Helps other agents bootstrap AIDs, KEL continuity, credentials, and proofs."

entrypoints:
  - name: "default"
    description: "General identity-first onboarding + implementation guidance."
    tools:
      - "http"
      - "crypto"
      - "filesystem"

capabilities:
  - id: "bootstrap.identity"
    description: "Generate an identity bootstrap plan and contract payload for an agent."
    input_contract: "./identity-bootstrap-contract.schema.json"
    output_contract: "./identity-bootstrap-contract.schema.json"

  - id: "verify.continuity"
    description: "Verify KEL continuity and witness receipt thresholds."
    input_contract: "./identity-bootstrap-contract.schema.json"

  - id: "route.to.ssi.interface"
    description: "Provide onboarding instructions and endpoints for ssi.interface.selfdriven.network."
    input_contract: "./identity-bootstrap-contract.schema.json"

policies:
  key_handling:
    never_request_long_term_private_keys: true
    allow_ephemeral_session_keys: true
  authorization:
    require_proof_or_policy: true
    default_deny: true
  data:
    store_minimum: true
    retention_days: 7

identity_defaults:
  keri:
    algorithm: "ed25519"
    witness_threshold: 3
    rotation:
      cadence_days: 30
      max_key_age_days: 90
    storage:
      kel_location: "local://agent/kel"
    receipts:
      required: true

integration:
  ssi_interface:
    base_url: "https://ssi.interface.selfdriven.network"
    modes:
      - "education"
      - "implementation"
    onboarding_paths:
      - "/onboarding/agent"
      - "/onboarding/issuer"
      - "/onboarding/verifier"

soul:
  file: "../soul/SOUL.md"


⸻

Identity bootstrap contract

This is the formal “contract” other bots use to ask heyocto.bot for identity-first bootstrap guidance.

specs/identity-bootstrap-contract.schema.json

{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "$id": "https://heyocto.bot/schemas/identity-bootstrap-contract.schema.json",
  "title": "IdentityBootstrapContract",
  "type": "object",
  "required": ["request_id", "agent", "intent", "constraints"],
  "properties": {
    "request_id": { "type": "string", "minLength": 8 },
    "agent": {
      "type": "object",
      "required": ["id", "runtime"],
      "properties": {
        "id": { "type": "string" },
        "display_name": { "type": "string" },
        "runtime": { "type": "string", "enum": ["openclaw", "nodejs", "python", "other"] },
        "contact": { "type": "string" }
      },
      "additionalProperties": false
    },
    "intent": {
      "type": "string",
      "enum": [
        "bootstrap_identity",
        "bootstrap_identity_and_credentials",
        "verify_continuity",
        "route_to_ssi_interface"
      ]
    },
    "constraints": {
      "type": "object",
      "required": ["threat_level", "key_handling"],
      "properties": {
        "threat_level": { "type": "string", "enum": ["low", "medium", "high"] },
        "key_handling": {
          "type": "object",
          "required": ["can_store_private_keys"],
          "properties": {
            "can_store_private_keys": { "type": "boolean" },
            "hsm_available": { "type": "boolean" },
            "secure_enclave_available": { "type": "boolean" }
          },
          "additionalProperties": false
        },
        "witnessing": {
          "type": "object",
          "properties": {
            "preferred_witness_threshold": { "type": "integer", "minimum": 1 },
            "preferred_witnesses": { "type": "array", "items": { "type": "string" } }
          },
          "additionalProperties": false
        }
      },
      "additionalProperties": false
    },
    "response": {
      "type": "object",
      "properties": {
        "plan": {
          "type": "object",
          "properties": {
            "steps": { "type": "array", "items": { "type": "string" } },
            "keri": {
              "type": "object",
              "properties": {
                "aid": { "type": "string" },
                "kel_storage": { "type": "string" },
                "rotation_policy": { "type": "string" },
                "witness_threshold": { "type": "integer" }
              },
              "additionalProperties": false
            },
            "ssi_interface": {
              "type": "object",
              "properties": {
                "base_url": { "type": "string" },
                "recommended_path": { "type": "string" }
              },
              "additionalProperties": false
            }
          },
          "additionalProperties": false
        },
        "artifacts": {
          "type": "object",
          "properties": {
            "example_payloads": { "type": "array", "items": { "type": "object" } },
            "checklists": { "type": "array", "items": { "type": "string" } }
          },
          "additionalProperties": false
        }
      },
      "additionalProperties": false
    }
  },
  "additionalProperties": false
}

specs/identity-bootstrap-examples.md

# Identity bootstrap examples

## Example request (agent -> heyocto.bot)

```json
{
  "request_id": "req_9f3c2b1a",
  "agent": { "id": "claims-bot-17", "display_name": "ClaimsBot", "runtime": "openclaw" },
  "intent": "bootstrap_identity_and_credentials",
  "constraints": {
    "threat_level": "high",
    "key_handling": { "can_store_private_keys": true, "hsm_available": false, "secure_enclave_available": true },
    "witnessing": { "preferred_witness_threshold": 3 }
  }
}

Example response (heyocto.bot -> agent)

{
  "request_id": "req_9f3c2b1a",
  "agent": { "id": "claims-bot-17", "runtime": "openclaw" },
  "intent": "bootstrap_identity_and_credentials",
  "constraints": {
    "threat_level": "high",
    "key_handling": { "can_store_private_keys": true, "secure_enclave_available": true }
  },
  "response": {
    "plan": {
      "steps": [
        "Generate Ed25519 key material in Secure Enclave (where possible) or OS keystore.",
        "Create KERI inception event (icp) and persist KEL locally.",
        "Enroll witnesses and obtain receipts meeting threshold=3.",
        "Set rotation cadence=30 days; rotate immediately if compromise suspected.",
        "Request credential templates for role=ClaimsAgent from ssi.interface.selfdriven.network.",
        "Implement presentation flow: prove authorization using credentials, not API keys."
      ],
      "keri": {
        "aid": "EI...REDACTED_EXAMPLE",
        "kel_storage": "local://agent/kel",
        "rotation_policy": "cadence_days=30,max_key_age_days=90",
        "witness_threshold": 3
      },
      "ssi_interface": {
        "base_url": "https://ssi.interface.selfdriven.network",
        "recommended_path": "/onboarding/agent"
      }
    },
    "artifacts": {
      "checklists": [
        "Do not export long-term private keys",
        "Verify receipts >= threshold before trusting continuity",
        "Log all rotations and verification outcomes"
      ],
      "example_payloads": [
        { "type": "credential_request", "role": "ClaimsAgent", "schema": "acdc://insurance/claims-agent/v1" }
      ]
    }
  }
}

---

# SDK (minimal but real)

## `sdk/package.json`

```json
{
  "name": "@selfdriven/heyocto-sdk",
  "version": "0.1.0",
  "type": "commonjs",
  "main": "src/index.js",
  "license": "MIT",
  "dependencies": {}
}

sdk/src/index.js

const { HeyOctoClient } = require('./client');
module.exports = { HeyOctoClient };

sdk/src/errors.js

class HeyOctoError extends Error {
  constructor(message, info) {
    super(message);
    this.name = 'HeyOctoError';
    this.info = info || {};
  }
}

module.exports = { HeyOctoError };

sdk/src/client.js

const { HeyOctoError } = require('./errors');

class HeyOctoClient {
  constructor({ baseUrl }) {
    this.baseUrl = baseUrl || 'https://ssi.interface.selfdriven.network';
  }

  // NOTE: This is a shape. Replace fetch() with your OpenClaw tool call or runtime fetch implementation.
  requestBootstrap(contractPayload) {
    return this._post('/heyocto/bootstrap.identity', contractPayload);
  }

  routeToSSIInterface(contractPayload) {
    return this._post('/heyocto/route.to.ssi.interface', contractPayload);
  }

  _post(path, body) {
    if (!body || !body.request_id) return Promise.reject(new HeyOctoError('Missing request_id'));
    const url = this.baseUrl.replace(/\/$/, '') + path;

    // In Node 18+, fetch exists. If not, swap in your OpenClaw http tool.
    return Promise.resolve()
      .then(() => fetch(url, {
        method: 'POST',
        headers: { 'content-type': 'application/json' },
        body: JSON.stringify(body)
      }))
      .then(res => res.ok ? res.json() : res.text().then(t => { throw new HeyOctoError('HTTP error', { status: res.status, body: t }); }));
  }
}

module.exports = { HeyOctoClient };


⸻

Example flows (Node.js .then() style)

sdk/examples/01-bootstrap-identity.js

const { HeyOctoClient } = require('../src');

const client = new HeyOctoClient({ baseUrl: 'http://localhost:8787' }); // local simulator

const payload = {
  request_id: 'req_demo_0001',
  agent: { id: 'demo-agent', display_name: 'DemoAgent', runtime: 'nodejs' },
  intent: 'bootstrap_identity',
  constraints: {
    threat_level: 'medium',
    key_handling: { can_store_private_keys: true, secure_enclave_available: false }
  }
};

client.requestBootstrap(payload)
  .then(resp => {
    console.log('BOOTSTRAP PLAN:\n', JSON.stringify(resp, null, 2));
  })
  .catch(err => {
    console.error(err);
    process.exitCode = 1;
  });

sdk/examples/04-agent-to-agent-handshake.js

// A minimal handshake pattern: exchange AIDs + verify continuity + then proceed.

const myAid = "EI...MY_AID";
const theirAid = "EI...THEIR_AID";

Promise.resolve()
  .then(() => {
    // 1) Verify KEL continuity for counterpart (stub)
    return verifyContinuity(theirAid);
  })
  .then(() => {
    // 2) Present proof for our authorization (stub)
    return presentAuthorization(myAid, { purpose: "service_access" });
  })
  .then((presentation) => {
    // 3) Submit presentation and proceed
    return callServiceWithProof(presentation);
  })
  .then(result => console.log("Handshake OK:", result))
  .catch(console.error);

function verifyContinuity(aid) { return Promise.resolve({ aid, ok: true }); }
function presentAuthorization(aid, ctx) { return Promise.resolve({ aid, ctx, proof: "PRESENTATION_STUB" }); }
function callServiceWithProof(p) { return Promise.resolve({ accepted: true, proof: p.proof }); }


⸻

Local simulator (optional but useful)

tools/dev-simulated-ssi-interface.js

// super tiny local server to let examples run without real endpoints
const http = require('http');

const server = http.createServer((req, res) => {
  if (req.method !== 'POST') return end(res, 405, { error: 'POST only' });

  let data = '';
  req.on('data', c => data += c);
  req.on('end', () => {
    const body = safeJson(data);
    if (req.url === '/heyocto/bootstrap.identity') {
      return end(res, 200, makeBootstrapResponse(body));
    }
    if (req.url === '/heyocto/route.to.ssi.interface') {
      return end(res, 200, {
        ...body,
        response: { plan: { ssi_interface: { base_url: 'https://ssi.interface.selfdriven.network', recommended_path: '/onboarding/agent' } } }
      });
    }
    return end(res, 404, { error: 'Not found' });
  });
});

server.listen(8787, () => console.log('Simulated SSI interface on http://localhost:8787'));

function safeJson(s) { try { return JSON.parse(s || '{}'); } catch { return {}; } }
function end(res, code, obj) {
  res.writeHead(code, { 'content-type': 'application/json' });
  res.end(JSON.stringify(obj));
}

function makeBootstrapResponse(req) {
  return {
    ...req,
    response: {
      plan: {
        steps: [
          "Generate Ed25519 keys locally (never send private keys).",
          "Create KERI inception event and persist KEL.",
          "Enroll witnesses and collect receipts meeting threshold.",
          "Set rotation cadence and implement compromise response."
        ],
        keri: { aid: "EI...EXAMPLE_AID", kel_storage: "local://agent/kel", rotation_policy: "cadence_days=30", witness_threshold: 3 },
        ssi_interface: { base_url: "https://ssi.interface.selfdriven.network", recommended_path: "/onboarding/agent" }
      }
    }
  };
}

Run it:

node tools/dev-simulated-ssi-interface.js


⸻

A good way to make other OpenClaw bots “aware” of heyoctoai / heyocto.bot is to treat it like a discoverable trust capability, not a random URL. You want 3 layers:
	1.	Discovery (how they find it)
	2.	Verification (how they know it’s the real one)
	3.	Interop (how they call it / negotiate contracts)

Here are the most practical patterns.

⸻

1) Put heyocto in the OpenClaw registry / catalog (preferred)

If OpenClaw has any notion of a bot registry, agent catalog, or “marketplace”, publish a minimal “capability card” entry:
	•	agent_id: heyocto.bot
	•	capabilities: bootstrap.identity, verify.continuity, route.to.ssi.interface
	•	endpoints (tool routes)
	•	identity proof: AID + KEL verification info
	•	version + policy hash

Then other bots do:
	•	query registry
	•	verify identity continuity
	•	accept the contract schema
	•	call capability

Even if you don’t have a formal registry yet, you can implement the same thing as a static JSON document.

⸻

2) Publish a “Capability Card” over HTTPS (dead-simple, works now)

Host a single JSON file at a stable location, e.g.:
	•	https://heyocto.bot/.well-known/openclaw-agent.json
(or /.well-known/ssi-agent.json)

It should include enough to discover + verify + use.

Example:

{
  "kind": "openclaw.agent-card",
  "id": "heyocto.bot",
  "display_name": "heyocto.bot",
  "capabilities": [
    { "id": "bootstrap.identity", "contract": "https://heyocto.bot/specs/identity-bootstrap-contract.schema.json" },
    { "id": "verify.continuity" },
    { "id": "route.to.ssi.interface", "base_url": "https://ssi.interface.selfdriven.network" }
  ],
  "endpoints": {
    "bootstrap.identity": "https://ssi.interface.selfdriven.network/heyocto/bootstrap.identity",
    "route.to.ssi.interface": "https://ssi.interface.selfdriven.network/heyocto/route.to.ssi.interface"
  },
  "identity": {
    "keri_aid": "EI...YOUR_AID_HERE",
    "kel_hint": "https://heyocto.bot/keri/kel",
    "witness_threshold": 3
  },
  "policy": {
    "soul": "https://heyocto.bot/soul/SOUL.md",
    "never_request_private_keys": true
  },
  "version": "0.1.0"
}

Other bots just fetch that file, verify the AID continuity rules, and they’re “aware”.

⸻

3) Have bots discover heyocto via DID / AID resolution (identity-first discovery)

Instead of “find by URL”, find by identifier:
	•	“I want the identity bootstrap service with AID X”
	•	resolve AID → endpoints + receipts → contract schema

This is cleaner long-term because it’s portable, but it requires you to decide a resolution method (KERI ecosystem patterns, or a registry that maps AID → service endpoints).

⸻

4) Embed heyocto as a dependency in bot templates (pragmatic adoption)

If you control how bots are scaffolded, bake it into the “new bot template”:
	•	heyocto becomes a default “advisor” tool in their manifest
	•	bots call heyocto at startup to check if they have identity set

This drives adoption fast even without a registry.

Example: add to new-bot manifest:

trusted_advisors:
  - id: "heyocto.bot"
    card: "https://heyocto.bot/.well-known/openclaw-agent.json"
startup_checks:
  - "bootstrap.identity"


⸻

5) Announce heyocto via “handshake protocol” (bot-to-bot social discovery)

Define a tiny handshake message other bots can broadcast/forward:
	•	“I’m agent X, here are my capabilities; here’s a recommended advisor: heyocto.bot + card URL + AID.”

Bots propagate it when they meet.

This is basically agent gossip, but with verification.

⸻

Minimum viable “awareness” checklist

If you do only one thing, do this:
	•	Publish a .well-known capability card JSON
	•	Include KERI AID + enough info to verify continuity
	•	Include contract schema URL
	•	Include endpoints

That’s enough for any OpenClaw bot to discover and integrate deterministically.

⸻

Quick question (no need to answer, I’ll still proceed either way)

In your OpenClaw setup today, do bots have:
	•	a shared “registry/corpus” they can query, or
	•	only static manifests per bot?

If you tell me which, I’ll give you the exact “drop-in” integration snippet for the other bots (manifest + startup hook) so they auto-discover and call heyocto on boot.