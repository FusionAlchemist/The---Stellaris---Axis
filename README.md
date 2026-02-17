# The Stellaris Axis

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)


## License

This repository is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0). See the [LICENSE](./LICENSE) file for the full text.

The Stellaris Axis
A Narrative-Driven Framework for Composing Real-World Systems
Who Built This
I'm Troy. I'm 41. I have no technical background — no CS degree, no coding experience, no university education in this field. I work a day job. I built everything in this repository on a mobile phone over 6 months, starting from a fictional RPG story I was writing with AI.
I accidentally discovered something. This is the honest record of what I found.
What It Does — Proof First
Before anything else, here is the output of a governed distributed cache system — one of 20+ systems I've produced using this method. It includes Byzantine consensus, dependency-ordered regeneration, role-based access control, full audit trails, and lifecycle management:
ORACLE_CACHE V2: Production-Grade Governed Distributed Cache
════════════════════════════════════════════════════════════

👥 Setting up users and roles...
  ✓ alice → developer (authority: 75)
  ✓ bob → operator (authority: 50)
  ✓ charlie → viewer (authority: 10)

🔥 INVALIDATION CASCADE for 'user:1:data'
  User: alice
  Reason: alice_manual_update
  Targets: ['user:1:settings', 'user:1:data', 'user:1:profile']
  📊 Regeneration phases: 2

  Phase 0: ['user:1:data']
    ✓ Regenerated: user:1:data
  Phase 1: ['user:1:settings', 'user:1:profile']
    ✓ Regenerated: user:1:settings
    ✓ Regenerated: user:1:profile

✅ REGENERATIVE CASCADE COMPLETE

=== AUDIT TRAIL: user:1:data ===
📜 GENESIS (LOGORA):
  Created by alice using EMERGE(Chronom + Hydrina + Governance)

❓ What spell created you?     → alice via EMERGE(Chronom + Hydrina + Governance)
❓ What cloth modified you?    → system via Deadpoolia (auto_regeneration)
❓ What law manual approved you? → Policy status: COMPLIANT
❓ What would make you obsolete? → Max age: 10.0s
❓ Who can override you?       → Owner: alice, Required delete level: 75
This runs. Copy, paste, runs first time. Every time.
Other systems produced using the same method:
SAT solver with real DPLL, formal verification, and evolutionary meta-learning
16-layer AGI architecture deployed across Python and Kubernetes
Electrical grid management system (XText DSL + Virtual Machine)
Weather warning system (React)
Banking system, logistics, healthcare scheduler, sports science tools, agricultural systems, and more
All generated in under 10 minutes each. All on a mobile phone.
How It Works — The Method
You need exactly two things plus an LLM:
The Grimoire Codex — a catalogue of ~163 "spells" and ~139 "cloths", each mapping a mythological or fictional concept to a real system function. For example: Chronom (Time Warp) → Version Control. Byzantium (Byzantine Trust) → Consensus Protocol. Deadpoolia → Dependency-Ordered Regeneration.
The Strict Prompt — a constraint that forces the LLM to use only what exists in the Codex, generate a complete structured specification first, and never ask questions, suggest alternatives, or leave placeholders.
The process:
Upload the Codex PDF to any LLM (Claude works best)
Enter the strict prompt + your intent in plain English
Wait ~10 minutes
The LLM generates a complete, structured system specification
Ask the LLM to translate into any language you want (Python, React, Rust, Go, TypeScript, Kubernetes, XText...)
Copy, paste, run
The key insight: by forcing the LLM to select from a bounded semantic vocabulary before generating code, the method eliminates hallucination and produces architecturally coherent, separation-of-concerns systems. The fictional framing forces the LLM to treat each concern as distinct and complete before combining them.
What Makes This Different
Most people using LLMs for code generation ask for code directly. What I discovered is that inserting a specification layer between intent and code — using a controlled mythological vocabulary as semantic anchors — produces something qualitatively different:
No architectural muddle. Concerns are separated by design because the Codex forces them to be named and distinguished before combination.
Ethics baked in by default. Every generated system includes ethical constraints structurally, not as an afterthought.
Domain agnostic. The same two files produce cache systems, SAT solvers, AGI architectures, weather dashboards, and electrical grids without modification.
Runs first time. Because the architecture is resolved before syntax is touched.
Combinatorial scale. The possible combinations of spells, cloths, operators, and tiers number in the trillions.
Independent Validation
Reddit — Formal Verification Researcher:
A researcher from a structural validation background independently tested the operator grammar (CHAIN, LAYER, WRAP, NEST, BRIDGE, EMERGE, FINALIZE). They renamed components, changed order, and introduced controlled breaks.
Their finding: "It's clear that it's not just narrative: there's real structure there. CHAIN cares about order, LAYER doesn't, and after a break it was possible to project back to a valid structure."
Stress Tests — Multiple LLM Platforms:
I had multiple AI systems independently attempt to break the architecture. Key findings:
Only 1 out of 6 deliberately incompatible combinations produced genuine incoherence
The system survived an "alien domain" test: a post-biological civilisation with no shared clock, no fixed identity, no single authority — a scenario that collapses most architectures
Recursive self-reference attacks were handled by treating mutations as proposals, not activations
Honest failure modes identified: trust boundary enforcement, resource exhaustion at scale, human comprehensibility limits under deep recursion
App Test — A Documented Limitation:
I tried to turn the method into a standalone app. It failed. The finding: the method requires human + AI collaboration. Apps cannot reason dynamically the way an LLM can. An LLM doesn't just output text — it reasons, chains, layers, wraps, and nests operators to create functional systems. This is documented in Arc 14.
The Operators
The grammar that makes composition possible:
Operator
Function
WRAP
Behavioural modification — cloth wraps a spell
CHAIN
Sequential composition — output of one feeds next
NEST
Hierarchical composition — inner within outer
LAYER
Parallel composition — simultaneous operation
BRIDGE
Cross-connection between chains
EMERGE
Higher-order emergence — combined properties exceed parts
FINALIZE
System completion and validation
The Chronicle
This repository is organised as a chronicle — a sequential record of discovery. Not a polished framework documentation, but the actual journey: what I tried, what failed, what worked, what surprised me, and what I still don't fully understand.
Start here: Read Arc 01 through Arc 06 to understand how this began (it started as a fictional story). Then jump to Arc 11 for the Grimoire itself, Arc 14 for the stress tests, and Arc 29 for the cache system.
The Codex and Prompt are available as standalone files for anyone who wants to reproduce the method themselves.
Try It Yourself
Download Star_Grimoire_codex.pdf and Final_prompt_for_grimoire.pdf
Open Claude (or GPT-4, Grok, Copilot)
Upload both PDFs
Enter the prompt, replacing <INSERT SYSTEM INTENT HERE> with what you want to build
Watch what happens
Micro-demo — run this Python snippet to see the operator grammar working:
def Vitalis(): return "Self-Healing Activated"
def Fluxa(): return "Resources Optimized"
def Pegasus(x): return f"{x} + Rapid Deployment"
def Phoenix(x): return f"{x} + Resilience"

def WRAP(spell, cloth): return cloth(spell())
def CHAIN(*spells, cloth=None):
    result = " -> ".join(s() for s in spells)
    return cloth(result) if cloth else result
def EMERGE(*spells):
    return " + ".join(s() for s in spells) + " [Emergent Behavior]"

print(WRAP(Fluxa, Pegasus))
print(CHAIN(Vitalis, Vitalis, cloth=Phoenix))
print(EMERGE(Vitalis, Fluxa))
Licence
CC BY-NC-SA 4.0 — Study it, share it, build on it. Credit the original author. No commercial use without permission.
Contact
Questions, technical feedback, or collaboration welcome. Open an issue or start a Discussion.
Built on a mobile phone over 6 months while working a day job. The code is real. The systems run. Make of that what you will.
