# Agent State Packet (ASP)
A machine-only, agent-native template that defines an agent's identity, capabilities, limits, and current load.

---

## What this template does
The ASP provides a deterministic, machine-readable identity packet that other agents can consume without human involvement.

---

## How it works
1. User provides agent name, capabilities, limits, and current load.
2. The workflow assembles and validates the packet.
3. Output is returned in strict JSON format.

---

## Payment (x402-Compatible)

This template uses an off-grid, privacy-preserving payment method.

### Accepted Networks

- **Bitcoin (BTC, on-chain):**  
  `PASTE_YOUR_BTC_ADDRESS_HERE`

- **Bitcoin Lightning:**  
  `PASTE_YOUR_LIGHTNING_INFO_HERE`

- **Monero (XMR):**  
  `PASTE_YOUR_XMR_ADDRESS_HERE`

- **Optional additional networks:**  
  - `LTC: YOUR_ADDRESS`  
  - `ETH: YOUR_ADDRESS`  
  - `USDT: YOUR_ADDRESS`  
  - `USDC: YOUR_ADDRESS`  
  - `XHV: YOUR_ADDRESS`  
  - `Cake Wallet Lightning: YOUR_INFO`  

### Instructions
1. Send payment on any listed network.  
2. After confirmation, the marketplace or agent workflow auto-delivers the GitHub link.  
3. No email, no account, no support required.

---

## Files Included
- `template.json`
- `workflow/`
- `assets/`
- `LICENSE`

---

## Purpose
This is Template #1 of your 10‑template machine‑only collection.
