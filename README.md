# 8x8 Agent Audio Readiness Check

A branded, customer-facing diagnostic page that verifies an agent's headset and microphone are fully ready before going Available in 8x8 Agent Workspace. Built to address the one-way audio race condition documented in VCC-183776.

## What It Checks

1. **Microphone Permission** — confirms the browser has mic access granted
2. **Audio Input Devices** — enumerates all detected microphones, highlights the active default
3. **Audio Output Devices** — lists all speakers and headsets
4. **Live Mic Signal** — 5-second live level meter to confirm the mic is transmitting
5. **Device Readiness Speed** — measures enumeration time against the 7-second risk window

Usage

Agents should open this page in Chrome each morning before their shift, click **Run Checks**, and wait for the green "You're good to go" result before setting their status to Available in Agent Workspace.

---

© 2026 8x8, Inc.
