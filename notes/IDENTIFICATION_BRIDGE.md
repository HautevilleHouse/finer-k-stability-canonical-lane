# Identification Bridge

Canonical wording: `endpoint identification / boundary object / final margin`.

In-paper anchor: `paper/FINER_K_STABILITY_PREPRINT.md` (bridge and final strict margin).

## Goal
Identify the canonical endpoint representative with the ordinary problem-side target for `proving persistence of refined K-stability and test-configuration control through an admissible stability-refinement closure architecture`.
This is the boundary/global-object step in the public Canonical Lane package.

## Objects

- canonical endpoint representative: the surviving endpoint object produced by the gate chain.
- problem-side target: the ordinary mathematical target statement named in the main preprint.
- endpoint lock: the transfer constraint used to identify the two descriptions.
- coherence remainder: the residual channel that must stay explicit through the final margin.

## Determining Class

The determining class is the collection of observables, locks, or transfer constraints declared by the main preprint and constants registry. In the older wording this appears as an `endpoint lock`; in the canonical wording it is endpoint identification.

## Closure Criterion

The bridge closes when:

1. the projected/core, transport, compactness, and rigidity gates have supplied their inputs;
2. the endpoint-transfer lock `stability_lock` identifies the surviving representative;
3. the coherence remainder `eps_coh` is not smuggled into the endpoint;
4. the strict closure margin `M_FKS` remains positive.

## Lemma Chain and Proof Payload

### Lemma ID.1 (lock persistence)
Endpoint locks persist along the admissible extracted lane when the transport and compactness gates have closed.

Payload: check `stability_lock` against the constants registry and runtime certificate.

### Lemma ID.2 (determining-class uniqueness)
Two admissible endpoint representatives that agree on the declared determining locks are equivalent under the repo's declared endpoint equivalence.

Payload: compare the main preprint's target statement with the bridge language in this file.

### Theorem ID.3 (coherence/identification closure)
If lock persistence, determining-class uniqueness, and strict coherence hold, then the endpoint representative is identified and the final margin `M_FKS` is meaningful.

## Current Instantiation

- endpoint-transfer artifact key: `stability_lock`
- coherence artifact key: `eps_coh`
- margin: `M_FKS`
- canonical equivalent: `endpoint identification / boundary object / final margin`
- audit surface: `repro/run_repro.sh`, `repro/certificate_runtime.json`, and `artifacts/constants_registry.json`
