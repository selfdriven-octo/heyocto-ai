# OpenClaw Manifest / Config — HeyOctoAI Integration

## Identity Provider
heyocto.bot

---

## Required Skills
- heyocto.identity.enablement

---

## Example openclaw.json

```json
{
  "agent": {
    "name": "example-agent",
    "identity_provider": "heyocto.bot",
    "skills": [
      "heyocto.identity.enablement"
    ]
  },
  "identity": {
    "keri": {
      "enabled": true,
      "auto_bootstrap": true,
      "witnesses": [
        "https://witness1.example",
        "https://witness2.example"
      ]
    }
  },
  "ssi": {
    "interface_url": "https://ssi.interface.selfdriven.network",
    "auto_register": true
  },
  "security": {
    "require_identity_before_network": true,
    "require_proof_for_privileged_actions": true
  }
}