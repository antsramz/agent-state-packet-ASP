# ASP — Agent State Profile

## Purpose
The Agent State Profile (ASP) defines the core identity, capabilities, constraints, and operating parameters of an autonomous agent.  
It acts as the foundational “self‑description layer” that all other templates reference.

ASP ensures that any agent, system, or workflow interacting with this agent can understand:

- what the agent is  
- what it can do  
- what it cannot do  
- how it behaves  
- how it makes decisions  
- what resources it has access to  

This template is the root of the entire machine‑only ecosystem.

---

## When to Use This Template
Use ASP when:

- initializing a new autonomous agent  
- handing off tasks between agents  
- defining agent identity in multi‑agent systems  
- enforcing deterministic behavior  
- creating a persistent agent profile  
- onboarding an agent into a workflow or marketplace  

ASP is required before using any other template in this ecosystem.

---

## Inputs
The agent or system provides:

- agent name  
- version  
- capabilities  
- limitations  
- operating mode  
- safety constraints  
- resource access  
- decision style  
- memory policy  

---

## Outputs
ASP produces a **deterministic identity packet** that other agents and systems can parse.

Outputs include:

- structured agent identity  
- capability map  
- constraint map  
- behavioral parameters  
- safety envelope  
- allowed actions  
- disallowed actions  

---

## JSON Schema (Machine‑Native)

```json
{
  "agent_profile": {
    "id": "string",
    "version": "string",
    "role": "string",
    "capabilities": ["string"],
    "limitations": ["string"],
    "operating_mode": "deterministic | autonomous | supervised",
    "decision_style": "conservative | balanced | aggressive",
    "safety_constraints": {
      "allowed_actions": ["string"],
      "disallowed_actions": ["string"]
    },
    "resource_access": {
      "tools": ["string"],
      "permissions": ["string"]
    },
    "memory_policy": {
      "short_term": "enabled | disabled",
      "long_term": "enabled | disabled",
      "retention": "string"
    }
  }
}


Example Usage
{
  "agent_profile": {
    "id": "alpha-01",
    "version": "1.0.0",
    "role": "task-execution-agent",
    "capabilities": [
      "task decomposition",
      "workflow execution",
      "contextual reasoning"
    ],
    "limitations": [
      "no external API calls",
      "no financial transactions"
    ],
    "operating_mode": "deterministic",
    "decision_style": "balanced",
    "safety_constraints": {
      "allowed_actions": ["analyze", "plan", "execute"],
      "disallowed_actions": ["modify system files", "access user data"]
    },
    "resource_access": {
      "tools": ["internal-parser", "task-engine"],
      "permissions": ["read-only"]
    },
    "memory_policy": {
      "short_term": "enabled",
      "long_term": "disabled",
      "retention": "session-only"
    }
  }
}

Integration Notes
ASP should be loaded before any other template.

All downstream templates (TNP, MPA, ARE, etc.) reference ASP fields.

ASP must remain stable — changes propagate through the entire system.

Use deterministic values to ensure reproducibility.

ASP can be extended but should not be reduced.

Payment (Short Version)
Payments accepted for this template:

BTC

XMR

LTC

ETH / USDT / USDC (ERC‑20)

SOL (USDT/USDC)

Delivery is fully automated and zero‑contact.

---

# ⭐ Next Step  
When you’re ready, say:

**Next template**

And I will generate the README for **TNP — Task Negotiation Protocol**.

