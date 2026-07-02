# EG2 Public Note (Capture and Restart)

Canonical wording: `transport / local-to-global transfer`.

In-paper anchor: `paper/FARRELL_JONES_CONJECTURE_PREPRINT.md` (`FJ_G2`).

## Goal
Expand the compressed capture/restart language into the local-to-global transport gate for `proving persistence of the `K`- and `L`-theoretic assembly package through an admissible geometric-group closure architecture`.

## Objects

- transport carrier: the admissible evolution, deformation, or routed lattice declared in the preprint.
- capture floor: `sigma_control`.
- restart law: the normalization/re-entry rule that keeps corrective steps inside the admissible class.
- carried losses: defect, restart, and normalization losses that must remain explicit.

## Closure Criterion

`FJ_G2` closes when `sigma_control` survives admissible losses and restart corrections: controlled defect stays above capture floor across admissible coarse losses.
This is the transport contribution to `M_FJ`.

## Lemma Chain and Proof Payload

### Lemma EG2.1 (transport accounting)
Every transport step used by the lane is charged to the declared defect ledger instead of being absorbed into prose.

Payload: check that the capture constant `sigma_control` is present in the constants registry and extraction inputs.

### Lemma EG2.2 (restart preservation)
Restart or normalization preserves the declared admissible class and keeps the remainder tracked.

Payload: inspect the repro script and guard output for the gate tied to `sigma_control`.

### Theorem EG2.3 (capture gate closure)
If transport accounting and restart preservation hold, then `FJ_G2` carries local control forward without breaking admissibility.

## Current Instantiation

- gate: `FJ_G2`
- artifact key: `sigma_control`
- canonical equivalent: `transport / local-to-global transfer`
- audit surface: `repro/run_repro.sh` and `repro/certificate_runtime.json`
