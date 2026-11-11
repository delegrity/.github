# Delegrity

**The authority layer between AI agents and your business systems.**

AI agents can now change real things: a supplier's bank account, a customer
record, an email to a client. Delegrity makes sure every such change is
allowed, approved by the right person when it matters, done exactly once, and
proven afterwards.

## The problem

An agent's access is not the same as its authority. A token tells a system
*who* is calling. It does not say *for whom* the agent acts, *what* it may do,
or whether that is still true today. The employee who set up the agent may have
left. The approval may have been for a different amount. The request may have
changed after someone said yes.

## How Delegrity works

Every consequential action follows one path:

1. **An agent asks.** It proposes an action instead of calling the target
   system directly.
2. **Authority is checked.** Who the agent acts for, under which mandate, within
   which limits.
3. **Your policy decides.** Delegrity asks your policy engine. Your rules stay
   yours.
4. **A person approves when needed.** The approval is bound to the exact
   request. If anything changes afterwards, the approval no longer counts.
5. **It runs once.** A single-use grant lets a runtime bridge perform exactly
   the approved action. The agent never holds the credentials.
6. **The result is proven.** The target is read back, and a signed receipt over
   a hash-chained record shows what was asked, decided and done.

If something goes wrong, people can stop an agent, a mandate or everything at
once, and the stop takes effect before the next side effect.

## What we build

- **Control API:** where agents ask and where the console reads.
- **Runtime bridge:** the only place an approved action is carried out.
- **Console:** where people see activity, approve requests, manage who may act
  for whom, and stop things fast.
- **SDKs and adapters:** Python and TypeScript, plus MCP, A2A and common agent
  frameworks.
- **Independent verifier:** checks receipts without trusting the rest of the
  system.

## Status

Delegrity is in **private preview**. It runs end to end and is tested on every
release, but please read this honestly:

- There is no independent certification yet. Our testing is our own.
- There is no production customer evidence yet, so we make no enterprise-ready
  claim.
- No named vendor is connected, and none is implied.

## Learn more

Visit [delegrity.com](https://delegrity.com) to see the story, or to ask for a
session where we map one protected action together.
