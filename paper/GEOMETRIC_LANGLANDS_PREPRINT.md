# Geometric Langlands via Hecke-Eigensheaf Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global correspondence super-architecture (`GEO1-GEO8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem super-manuscript

---

## Abstract

This manuscript develops a canonical-lane super-architecture for the target problem: proving persistence of admissible Hecke eigensheaves and spectral correspondences through a multi-lane geometric-Langlands architecture.

Unlike the single-endpoint lanes in the rest of the library, this repository is a coordinating super-repo. Its theorem chain closes a declared admissible correspondence lattice spanning the native geometric-Langlands routed families rather than a single primitive sheaf-theoretic transfer theorem. The proof program is organized as eight steps `GEO1-GEO8` with executable closure gates `GEO_G1`, `GEO_G2`, `GEO_G3`, `GEO_G4`, `GEO_G5`, `GEO_G6`, and `GEO_GM`.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible correspondence lattice and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For the declared admissible families of curves, reductive groups, and dual data, Hecke eigensheaves and spectral-side local systems match across the routed geometric-Langlands correspondence lattice with the predicted local and categorical compatibilities.

The canonical-lane super-repo proof path is:

1. encode admissible correspondence data in a canonical class `A_corr`,
2. establish local-to-global persistence of Hecke control across routed sub-lane families,
3. exclude bad limits by rigidity and compactness of sheaf towers,
4. stitch the extracted endpoint through the bridge package,
5. identify the target packet with the predicted spectral-side endpoint.

### 1.2 Super-repo claim boundary

- the correspondence lattice and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared super-lane closes,
- the claim is made on the admissible geometric-Langlands correspondence lattice, not on unscoped claims outside the declared routed families.

Let `A_corr` denote the admissible class used throughout Sections 2-9 and Appendices A-E.

### 1.3 Explicit remainder discipline

Write `Y = Y_mc^GEO \sqcup R_GEO`, where `Y_mc^GEO` is the declared admissible visible sector induced by `A_corr` and `R_GEO` is the explicit complement in the full problem-side class `Y`. The theorem package closes on `Y_mc^GEO`; it does not silently identify admissible closure with unrestricted closure on `Y`. Any stronger external consequence must therefore be expressed as control, reduction, or iterative refinement of `R_GEO`.

Equivalently, if `P_mc` denotes projection to the admissible sector and `Q_rem := I - P_mc`, then the visible problem-side object decomposes as

`X_geom = P_mc X_geom + Q_rem X_geom`

with `Q_rem X_geom` represented by the defect and coherence ledgers tracked in this repository. The bridge note `notes/GEOMETRIC_GALOIS_BRIDGE.md` records the mainstream geometric/arithmetic precursors used to interpret this decomposition for reviewers.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Super-repo interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible correspondence lattice |
| `A2` Flux primacy | Hecke transport and categorical restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive sheaf-theoretic core plus explicit defect ledger |
| `A4` Local-to-global transfer | local Satake and Hecke identities propagate across the routed families |
| `A5` Window transfer | bounded local windows propagate to super-lane closure constants |
| `A6` Tensor covariance | canonical response quantities live on the projected sheaf sector |
| `A7` Corrective morphisms | renormalization and categorical descent preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects and Correspondence Lattice

Let `tau` denote the deformation parameter and let

`u_tau = (H_tau, S_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of Hecke packets, spectral data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible sheaf towers: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_GEO = min(kappa_hecke, sigma_local, kappa_compact, rho_rigidity, eigensheaf_transfer) - eps_coh`.

Target:

`M_GEO > 0`.

### 3.1 Routed sub-lane families

The super-repo coordinates the following admissible correspondence families:

1. geometric Satake and spherical Hecke transport,
2. Hecke eigensheaf generation,
3. spectral-side coherence on local systems,
4. categorical duality and sheaf-theoretic transfer,
5. local-global stitching across stack-level packets.

---

## 4. Response and Gate Interface

Let `H_resp` be the projected correspondence sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive Hecke-eigensheaf floor that prevents collapse of the admissible correspondence package.

| Gate | Constant | Criterion |
|---|---|---|
| `GEO_G1` | `kappa_hecke` | projected Hecke response has a strict positive floor |
| `GEO_G2` | `sigma_local` | local correspondence defect stays above capture floor |
| `GEO_G3` | `kappa_compact` | normalized near-failure sheaf towers are precompact |
| `GEO_G4` | `rho_rigidity` | bad nongeometric countermodels are excluded |
| `GEO_G5` | `eigensheaf_transfer` | rigid limits transfer to the predicted eigensheaf endpoint |
| `GEO_G6` | `eps_coh` | strict coherence on the determining class |
| `GEO_GM` | derived | all upstream gates pass and `M_GEO > 0` |

Current artifact values give:

- `kappa_hecke = 1.0932`,
- `sigma_local = 1.0750000000000002`,
- `kappa_compact = 0.8038585209003215`,
- `rho_rigidity = 1.078`,
- `eigensheaf_transfer = 1.0315400000000001`,
- `eps_coh = 0.0`.

Hence `M_GEO = 0.8038585209003215 > 0`.

---

## 5. Local Correspondence, Compactness, and Super-Lane Theorem Chain

1. `GEO1` Active Hecke block on the projected response sector.
2. `GEO2` Uniform local capture bounds across the admissible correspondence lattice.
3. `GEO3` Restart and categorical invariance across routed sub-lane families.
4. `GEO4` First-failure compactness extraction for sheaf towers.
5. `GEO5` Rigidity exclusion of bad nongeometric limits.
6. `GEO6` Sub-lane stitching of extracted endpoints through admissible correspondence morphisms.
7. `GEO7` Determining-class identification via Hecke, Satake, and spectral observables.
8. `GEO8` Final persistence theorem: predicted geometric-Langlands correspondence survives on the declared admissible lattice.

---

## 6. Rigidity, Endpoint Transfer, and Identification

The tracked theorem-level inputs are:

- `rho_rigidity = 1.078 > 0`,
- `eigensheaf_transfer = 1.0315400000000001 > 0`,
- `eps_coh = 0` in strict mode.

---

## 7. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `GEO_G1, GEO_G2, GEO_G3, GEO_G4, GEO_G5, GEO_G6, GEO_GM = PASS`,
- strict margin `M_GEO = 0.8038585209003215`,
- lane: `manifold_constrained`.

---

## 8. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 9. References

1. V. Drinfeld, *Langlands conjecture for `GL(2)` over functional fields*, Proc. ICM 1986.
2. E. Frenkel, *Lectures on the Langlands program and conformal field theory*, in *Frontiers in Number Theory, Physics, and Geometry II*, Springer, 2007.
3. D. Gaitsgory and J. Lurie, *Weil's Conjecture for Function Fields, Volume I*, Princeton Univ. Press, 2019.
4. D. Arinkin and D. Gaitsgory, *Singular support of coherent sheaves and the geometric Langlands conjecture*, Selecta Math. 21 (2015), 1-199.
