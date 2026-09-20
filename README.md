<div align="center">

<img src="./assets/profile-banner.svg" width="100%" alt="KyDoCia — Senior Roblox Gameplay & Systems Engineer" />

<br />

### Senior Roblox Gameplay & Systems Engineer

**7+ years with Roblox Studio & Luau · Multiplayer Architecture · Combat · Security · Performance**

I engineer production systems where **game feel, authority, networking, security and maintainability** have to work together.

![Luau](https://img.shields.io/badge/Luau-1B1B1F?style=for-the-badge&logo=lua&logoColor=8B7CFF)
![Roblox Studio](https://img.shields.io/badge/Roblox_Studio-1B1B1F?style=for-the-badge&logo=robloxstudio&logoColor=8B7CFF)
![Rojo](https://img.shields.io/badge/Rojo-1B1B1F?style=for-the-badge&logo=roblox&logoColor=8B7CFF)
![Git](https://img.shields.io/badge/Git-1B1B1F?style=for-the-badge&logo=git&logoColor=8B7CFF)

</div>

---

## Engineering Profile

I specialize in Roblox systems that become difficult once a game leaves the prototype stage: **authoritative multiplayer gameplay, combat state, networking boundaries, exploit resistance, lifecycle correctness, persistence and performance**.

My approach is architecture-first but runtime-driven. A system is not finished because its modules look clean — it is finished when ownership is unambiguous, invalid state is rejected, cleanup is deterministic, failure modes are understood, and the complete gameplay loop survives repeated runtime execution.

```text
Client        -> input, prediction, presentation, feedback
Network       -> explicit contracts, validation, rate/abuse boundaries
Server        -> authority, state transitions, simulation, rewards
Persistence   -> schema discipline, lifecycle, failure-safe writes
Security      -> trust boundaries, evidence, layered detection
Runtime       -> profiling, observability, cleanup, regression gates
```

---

## Advanced Systems Work

<table>
<tr>
<td width="50%" valign="top">

### Real-Time Gameplay & Combat

- Server-authoritative combat architecture
- Parry / timing-window systems
- Target acquisition and combatant state
- Momentum and escalation mechanics
- Player + NPC combat abstractions
- Round lifecycle and deterministic cleanup
- Animation/gameplay synchronization
- Camera, feedback and responsiveness layers
- Cross-platform input architecture

</td>
<td width="50%" valign="top">

### Multiplayer & Security

- Explicit client/server trust boundaries
- Remote validation and exploit-resistant APIs
- Server-owned rewards and critical state
- Detection pipelines and evidence-oriented security
- Layered anti-exploit architecture
- State ownership and invariant enforcement
- Abuse-aware networking design
- Failure containment instead of client trust

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Architecture & Data

- Modular service/controller boundaries
- Shared domain abstractions
- Persistent player data architecture
- Versionable/configurable systems
- Lifecycle-safe initialization and teardown
- Dependency isolation
- Reusable gameplay infrastructure
- Refactoring without rewriting the product

</td>
<td width="50%" valign="top">

### Production Engineering

- Runtime-first validation in Roblox Studio
- Performance profiling and bottleneck analysis
- Regression-oriented development
- Git / branch / pull-request workflows
- Rojo-based project structure
- Technical documentation and handoff
- Maintainability under continued feature growth

</td>
</tr>
</table>

---

## How I Design Systems

```luau
-- The principle is simple:
-- presentation may live on the client;
-- truth does not.

Client:RequestAction(input)
        |
        v
Server:Validate(context, input)
        |
        +-- reject impossible / stale / abusive state
        |
        v
Domain:Transition(authoritativeState)
        |
        +-- replicate result
        +-- record evidence when relevant
        +-- guarantee cleanup
```

I prefer **explicit ownership, narrow interfaces and enforceable invariants** over large scripts held together by convention. Security is part of architecture, not a patch added after exploitation begins.

---

## Selected Engineering Domains

**Competitive combat** — precision mechanics, authoritative state, targeting, NPC/player parity, round orchestration and high-feedback gameplay.

**Security engineering** — modular anti-exploit systems built around server authority, behavioral signals, evidence and progressive response rather than fragile client-side checks.

**Persistent social/identity systems** — player data, collectibles, titles, profile/showcase state and UI-driven identity presentation with clear domain boundaries.

**Roleplay infrastructure** — interconnected vehicle ownership, permissions, economy, enforcement and persistence systems designed as one domain rather than isolated scripts.

> Some current systems and R&D repositories are intentionally private. Public code is not a complete representation of my production work.

---

## Engineering Standards

| Principle | Production meaning |
|---|---|
| **Authority** | The server owns decisions that affect competitive or economic truth. |
| **Security** | Every client-controlled boundary is treated as untrusted input. |
| **Correctness** | State transitions have explicit preconditions, ownership and cleanup. |
| **Performance** | Optimize measured bottlenecks; avoid architecture that creates unnecessary work. |
| **Scalability** | New content should extend systems, not require structural rewrites. |
| **Maintainability** | Another engineer should be able to reason about the system without reverse-engineering it. |
| **Observability** | Important failures should produce enough evidence to diagnose what happened. |

---

## Tooling

<div align="center">

![Luau](https://img.shields.io/badge/Luau-1B1B1F?style=flat-square&logo=lua&logoColor=8B7CFF)
![Roblox Studio](https://img.shields.io/badge/Roblox_Studio-1B1B1F?style=flat-square&logo=robloxstudio&logoColor=8B7CFF)
![Rojo](https://img.shields.io/badge/Rojo-1B1B1F?style=flat-square&logo=roblox&logoColor=8B7CFF)
![Git](https://img.shields.io/badge/Git-1B1B1F?style=flat-square&logo=git&logoColor=8B7CFF)
![GitHub](https://img.shields.io/badge/GitHub-1B1B1F?style=flat-square&logo=github&logoColor=8B7CFF)
![VS Code](https://img.shields.io/badge/VS_Code-1B1B1F?style=flat-square&logo=visualstudiocode&logoColor=8B7CFF)
![TypeScript](https://img.shields.io/badge/TypeScript-1B1B1F?style=flat-square&logo=typescript&logoColor=8B7CFF)

</div>

**Primary production stack:** Luau + Roblox Studio.  
**Workflow:** Git/GitHub + Rojo, with TypeScript/RobloxTS as an expanding part of the toolchain.

---

## What I Optimize For

```text
Correctness > cleverness
Server authority > client trust
Measured performance > premature optimization
Explicit state > hidden coupling
Reusable architecture > repeated implementation
Runtime evidence > assumptions
Product quality > code for code's sake
```

---

## Collaboration

I am interested in technically serious Roblox productions where engineering quality materially affects the product — particularly **competitive gameplay, combat, multiplayer architecture, security and complex systems**.

I work best on problems that require more than making a feature function: **making it reliable under real players, hostile clients, continued development and production constraints.**

<div align="center">

### Build the system so the next feature does not break the last one.

`Gameplay Engineering` · `Combat Systems` · `Multiplayer Architecture` · `Security` · `Performance`

</div>
