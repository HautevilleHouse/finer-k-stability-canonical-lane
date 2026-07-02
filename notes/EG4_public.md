# EG4 Public Note (Rigidity and Endpoint Transfer)

Canonical wording: `bad-limit exclusion / endpoint transfer`.

In-paper anchor: `paper/FINER_K_STABILITY_PREPRINT.md` (`FKS_G4` and `FKS_G5`).

## Goal
Separate the rigidity job from the endpoint-transfer job for `proving persistence of refined K-stability and test-configuration control through an admissible stability-refinement closure architecture`.
The older wording `rigidity and endpoint-transfer` corresponds to bad-limit exclusion plus the bridge into the intended endpoint object.

## Objects

- bad-limit class: candidates extracted by the compactness gate but incompatible with closure.
- rigidity floor: `rho_rigidity`.
- endpoint-transfer lock: `stability_lock`.
- coherence interface: `eps_coh` remains available to the bridge and final margin.

## Closure Criterion

`FKS_G4` closes when `rho_rigidity` excludes bad endpoint alternatives: bad endpoint alternatives are excluded by the rigidity monitor.
`FKS_G5` closes when `stability_lock` transfers the surviving endpoint to the intended target class: the rigid endpoint transfers to the intended problem-side class.
Together they feed the strict margin `M_FKS`.

## Lemma Chain and Proof Payload

### Lemma EG4.1 (bad-limit exclusion)
Every extracted bad limit contradicts a declared rigidity constraint or leaves the admissible class.

Payload: check `rho_rigidity` in the registry and certificate surfaces.

### Lemma EG4.2 (endpoint transfer)
The surviving rigid representative is locked to the standard problem-side endpoint by `stability_lock`.

Payload: read this note together with `notes/IDENTIFICATION_BRIDGE.md`.

### Theorem EG4.3 (rigidity/transfer gate closure)
If bad limits are excluded and the endpoint lock is active, then `FKS_G4` and `FKS_G5` deliver the boundary object needed by the final margin.

## Current Instantiation

- rigidity gate: `FKS_G4`
- rigidity artifact key: `rho_rigidity`
- transfer gate: `FKS_G5`
- transfer artifact key: `stability_lock`
- canonical equivalent: `bad-limit exclusion / endpoint identification`
- audit surface: `notes/IDENTIFICATION_BRIDGE.md` and `repro/certificate_runtime.json`
