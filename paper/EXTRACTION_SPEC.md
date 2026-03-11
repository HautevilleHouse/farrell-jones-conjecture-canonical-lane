# Constant Extraction Spec (FJ)

    This file defines the theorem-constant extraction contract for this repository.

    ## Objective

    1. extract raw constants from explicit component inputs and formulas,
    2. normalize by declared references,
    3. promote into `artifacts/constants_registry.json` and `artifacts/stitch_constants.json`.

    ## Inputs
    - `artifacts/constants_extraction_inputs.json`

    ## Outputs
    - `artifacts/constants_extracted.json`
    - `artifacts/constants_registry.json`
    - `artifacts/stitch_constants.json`
    - `artifacts/promotion_report.json`

    ## Formula Set
    - `kappa_assembly_raw = c_assembly_raw * assembly_density_raw - e_assembly_raw`
- `sigma_control_raw = control_floor_raw - coarse_loss_raw - restart_loss_raw`
- `kappa_compact_raw = 1.0 / (1.0 + delta_comp_sup_raw)`
- `rho_rigidity_raw = rho_rigidity_raw`
- `isomorphism_transfer_raw = c_iso_raw * transfer_gain_raw - e_iso_raw`
- `eps_coh_raw = eps_coh_raw`
- `sigma_star_can_raw = sigma_star_can_raw`

    ## Validations
    - positivity required for: `kappa_assembly`, `sigma_control`, `kappa_compact`, `rho_rigidity`, `isomorphism_transfer`, `sigma_star_can`
    - nonnegative required for: `eps_coh`
    - strict-zero required for: `eps_coh` in strict mode

    ## Execution
    `repro/run_repro.sh` runs:
    1. `scripts/extract_constants.py`
    2. `scripts/promote_constants.py`
    3. `scripts/fj_closure_guard.py`
