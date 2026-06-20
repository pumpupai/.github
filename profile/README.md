<div align="center">

# Pump Up

### The operations workspace for AI-augmented teams

Where AI agents drop work for humans — and humans approve, route, and decide.

[Website](https://pumpup.com) · [Docs](https://docs.pumpup.com) · [SDKs & Integrations](https://github.com/pumpupai/pumpup)

</div>

---

Ship an agent into production and it handles most of the work — but a human still has to approve, route, or decide on the slice it can't. **Pump Up is where that handoff lives.**

It's the control plane for the team processing the residual slice of agent work: reviewing, approving, routing, handling exceptions. One coherent surface — **queue → item view → audit log → manager view** — with an immutable record of who decided what and why. The agent declares the work; we render it beautifully and keep the receipts.

We're **agent-agnostic**: run agents from any vendor or your own, and Pump Up ingests work from all of them.

## How it works

- **📥 Queue** — every pending decision in one real-time, filterable list, with priority and SLA timers.
- **🗂️ Item view** — the decision surface, pre-loaded with all the context the agent gathered. Fast and keyboard-driven: approve, reject, edit-and-approve, or escalate.
- **📜 Audit log** — an append-only history of every decision, always on. The record your compliance team will ask for.
- **📊 Manager view** — throughput, SLA compliance, queue depth, override rates. Where the ops leader runs the team.

## Get started

Drop a human in the loop in about 20 lines:

```bash
pip install pumpup-sdk      # Python
npm install pumpup-sdk      # TypeScript
```

```ts
const decision = await pumpup.requestApproval({
  type: "refund_over_threshold",
  context: { customer, amount, agentRecommendation },
  sla: "4h",
  routingHint: { team: "claims" },
});
```

The human decides in a fast, purpose-built UI; your agent gets the answer back.

→ **[Read the docs](https://docs.pumpup.com)** · **[SDKs & integrations](https://github.com/pumpupai/pumpup)** (Python, TypeScript, OpenClaw — more by where developers build)

## Integrations

Building on an agent framework? Skip the wiring — first-class integrations live in [`pumpupai/pumpup`](https://github.com/pumpupai/pumpup), starting with **OpenClaw**.

---

<div align="center">

**[pumpup.com](https://pumpup.com)** — built for the teams handling what agents can't.

</div>
