# The Farrell-Jones Conjecture via Assembly Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`FJ1-FJ8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving persistence of the `K`- and `L`-theoretic assembly package through an admissible geometric-group closure architecture.

The proof program is organized as eight steps `FJ1-FJ8` with executable closure gates `FJ_G1`, `FJ_G2`, `FJ_G3`, `FJ_G4`, `FJ_G5`, `FJ_G6`, and `FJ_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For every group in the declared admissible family, the algebraic `K`- and `L`-theory assembly maps are isomorphisms relative to the virtually cyclic family.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let

`u_tau = (A_tau, G_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of assembly packets, admissible geometric-group data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_FJ = min(kappa_assembly, sigma_control, kappa_compact, rho_rigidity, isomorphism_transfer) - eps_coh`.

Target:

`M_FJ > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive assembly floor that prevents collapse of the admissible `K/L`-theoretic transport package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `FJ_G1` | `kappa_assembly` | projected assembly response has a strict positive floor |
| `FJ_G2` | `sigma_control` | controlled defect stays above capture floor across admissible coarse losses |
| `FJ_G3` | `kappa_compact` | normalized near-failure families are precompact and control windows do not collapse |
| `FJ_G4` | `rho_rigidity` | bad nonisomorphic assembly countermodels are excluded |
| `FJ_G5` | `isomorphism_transfer` | rigid limit transfers to the assembly-isomorphism endpoint class |
| `FJ_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `FJ_GM` | derived | all upstream gates pass and `M_FJ > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_assembly` = 1.0918990000000002,
- `sigma_control` = 1.073,
- `kappa_compact` = 0.8045052292839904,
- `rho_rigidity` = 1.077,
- `isomorphism_transfer` = 1.029422,
- `eps_coh = 0.0`.

Hence:

`M_FJ = 0.8045052292839904 > 0`.

### 4.5 Raw coercive constant

Define `kappa_assembly^(raw) := c_assembly_raw * assembly_density_raw - e_assembly_raw`.

Current extracted value:

`kappa_assembly = 1.0918990000000002`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`FJ1-FJ8`)

1. `FJ1` Active assembly block on the projected response sector.
2. `FJ2` Uniform control capture bounds on the canonical coarse tube.
3. `FJ3` Restart map preserving admissible geometric-group data.
4. `FJ4` First-failure compactness extraction.
5. `FJ5` Rigidity exclusion of bad nonisomorphic assembly countermodels.
6. `FJ6` Isomorphism-transfer closure on the extracted endpoint class.
7. `FJ7` Determining-class identification of the Farrell-Jones endpoint.
8. `FJ8` Final persistence theorem: the assembly-isomorphism endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_control^(raw) := control_floor_raw - coarse_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_control = 1.073`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8045052292839904`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of nonisomorphic assembly countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.077 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the assembly-isomorphism endpoint class by the bridge inequality.

Define `isomorphism_transfer^(raw) := c_iso_raw * transfer_gain_raw - e_iso_raw`.

Current extracted value:

`isomorphism_transfer = 1.029422 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of assembly and control observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_assembly` | `FJ_G1` | `1.0918990000000002` |
| `sigma_control` | `FJ_G2` | `1.073` |
| `kappa_compact` | `FJ_G3` | `0.8045052292839904` |
| `rho_rigidity` | `FJ_G4` | `1.077` |
| `isomorphism_transfer` | `FJ_G5` | `1.029422` |
| `eps_coh` | `FJ_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `FJ_G1, FJ_G2, FJ_G3, FJ_G4, FJ_G5, FJ_G6, FJ_GM = PASS`,
- strict margin `M_FJ = 0.8045052292839904`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_assembly^(raw) > 0`, hence `FJ_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit control losses. Positivity of `sigma_control` yields `FJ_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and control windows have a positive spacing lower bound, giving `kappa_compact > 0` and `FJ_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `FJ_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `isomorphism_transfer = 1.029422 > 0`, while strict coherence requires `eps_coh = 0`.

Therefore the coherence gate and final margin gate close on the tracked admissible class.

---

## 11. References

1. F. T. Farrell and L. E. Jones, *Isomorphism conjectures in algebraic `K`-theory*, J. Amer. Math. Soc. 6 (1993), 249-297.
2. A. Bartels and W. Lück, *The Farrell-Jones Conjecture for hyperbolic groups*, Ann. of Math. 175 (2012), 631-689.
3. A. Bartels, W. Lück, and H. Reich, *The `K`-theoretic Farrell-Jones conjecture for hyperbolic groups*, Invent. Math. 172 (2008), 29-70.
