# Formally Verified Proofs for Cyclic Continual Learning

Machine-checked Lean 4 certificates for two papers on spectrally optimal stepsizes in cyclic continual learning. All proofs verified via [Aristotle](https://aristotle.harmonic.fun) (Harmonic) against Mathlib commit `f897ebcf`.

## Papers

- **Paper 1:** "Closed-Form Optimal Stepsizes for Cyclic Continual Learning: The Complete d=2 Theory and the Algebraic Boundary at K=3"
- **Paper 2:** "Exponential Forgetting Decay via Spectral Stepsize Optimisation in Cyclic Continual Learning"

David G. Hanly, 2026. Independent Researcher.

## Numbers

| | Files | Theorems + Lemmas | `sorry` |
|---|---|---|---|
| Paper 1 | 49 | 517 | 0 |
| Paper 2 | 8 | 52 | 0 |
| Shared | 1 | 8 | 0 |
| **Total** | **58** | **577** | **0** |

## Repository Structure

```
paper1/          49 Lean 4 files — certificates for Paper 1
paper2/           8 Lean 4 files — certificates for Paper 2
shared/           1 Lean 4 file  — cited by both papers
```

Each file is named `{UUID}-output.lean` where the UUID matches the certificate identifier cited in the papers. Submit any UUID to [aristotle.harmonic.fun](https://aristotle.harmonic.fun) to retrieve the proof interactively.

## Verification

Every file satisfies:

```bash
# Zero sorry statements across the entire corpus
grep -r "sorry" paper1/ paper2/ shared/ | grep -v "-- " | wc -l
# 0
```

To verify independently: submit any `.lean` file to the Aristotle proof engine, or check against Lean 4 + Mathlib (commit `f897ebcf`).

## UUID Index — Paper 1

58 certificate entries across 49 files (some files contain multiple certificates).

| UUID | Key Theorems | Description |
|------|-------------|-------------|
| `21509db5` | `spectral_radius_optimal_K3_commutative` | Closed-form stepsizes, K=3 commutative |
| `a786aae7` | `master_quartic_exists`, `quartic_determines_stability` | The Master Quartic — first stability polynomial for K=3, d=2 |
| `097cb1f5` | `discriminant_boundary`, `rotational_phase_transition` | Rotational phase transition at T²=4D |
| `16894d9f` | `d2_miracle`, `palindromic_eigenvalue_identity` | The d=2 Miracle — structural identity for closed forms |
| `e9d96090` | `curriculum_theorem`, `trace_ordering_optimal` | Curriculum Theorem — optimal task ordering via traces |
| `c42f6769` | `conjE_K3`, `rayleigh_annihilation` | Conjecture E — Rayleigh quotient annihilation |
| `72f51b9b` | `bwt_formula` | Buridan's Wild Theorem formula |
| `bebabb9f` | `stability_margin_certificate` | Stability margin certificate |
| `809a46bf` | `cl_stability_certificate` | CL stability certificate |
| `047c9d5c` | `K4_convergence_certificate` | K=4 convergence certificate |
| `94b60764` | `K5_convergence_certificate` | K=5 convergence certificate |
| `6aedabda` | `robust_stability`, `elsner_spectral_perturbation` | Robust stability and Elsner bound |
| `1d68e65b` | `K2_optimal_stepsizes`, `K2_closed_form` | K=2 optimal stepsizes (extends Peng & Vidal 2025) |
| `aaccadcb` | `binary_tree_recursion`, `palindromic_structure` | Binary tree recursion chain for all K |
| `930812f2` | `neumann_resolvent`, `spectral_radius_bound` | Neumann series and resolvent bounds |
| `cc5d7699` | `jordan_iterate_bound`, `nilpotent_index_bound` | Jordan normal form iterate bounds |
| `b79ce7f3` | `chebyshev_node_computation`, `equioscillation` | Chebyshev polynomial infrastructure |
| `5f5999a6` | `polynomial_degree_bound`, `root_count_ivt` | Polynomial root counting via IVT |
| `292bc4d5` | `submultiplicativity`, `operator_norm_product` | Matrix norm submultiplicativity |
| `dc62d2aa` | `spectral_radius_continuous`, `gelfand_formula` | Spectral radius continuity |
| `f29328a1` | `abel_ruffini_obstruction` | Abel-Ruffini: no closed form for K≥3 general |
| `509556e5` | `K3_noncommutative_spectral_radius` | K=3 non-commutative spectral radius |
| `48d99d97` | `trace_det_invariants` | Trace and determinant invariants |
| `b0438fe2` | `cycle_operator_factorisation` | Cycle operator factorisation |
| `306119c7` | `contraction_mapping_convergence` | Contraction mapping convergence |
| `8a1bdec6` | `spectral_gap_lower_bound` | Spectral gap lower bound |
| `14470f51` | `eigenvalue_perturbation_bound` | Eigenvalue perturbation bound |
| `719c8d4f` | `lyapunov_function_construction` | Lyapunov function for cyclic GD |
| `d5aec6e4` | `polynomial_evaluation_at_matrix` | Polynomial evaluation at matrices |
| `ba9525b6` | `spectral_mapping_theorem` | Spectral mapping theorem |
| `e15ee141` | `submultiplicative_norm_bound` | Submultiplicative norm bound |
| `bda28350` | `jordan_block_power_bound` | Jordan block power bound |
| `89f3f01e` | `K3_discriminant_formula` | K=3 discriminant formula |
| `4c51e673` | `trace_power_identity` | Trace power identity |
| `abd10bab` | `neumann_convergence_criterion` | Neumann convergence criterion |
| `a5321b62` | `spectral_radius_product_bound` | Spectral radius product bound |
| `ef566474` | `characteristic_polynomial_K3` | Characteristic polynomial for K=3 |
| `f04a3e22` | `cycle_operator_trace_formula` | Cycle operator trace formula |
| `edb1428c` | `palindromic_spectrum` | Palindromic spectrum property |
| `8c0268ea` | `K2_commutative_closed_form` | K=2 commutative closed form |
| `10dc743d` | `stability_region_boundary` | Stability region boundary |
| `1100f846` | `convergence_rate_formula` | Convergence rate formula |
| `30475e78` | `optimal_stepsize_existence` | Optimal stepsize existence |
| `974a4dd6` | `spectral_radius_submultiplicative` | Spectral radius submultiplicativity |
| `94078188` | `K3_eigenvalue_formula` | K=3 eigenvalue formula |
| `ee5c879b` | `real_eigenvalue_criterion` | Real eigenvalue criterion |
| `1d60ff74` | `K2_global_minimiser` | K=2 global minimiser |
| `4f03368e` | `matrix_exponential_bound` | Matrix exponential bound |
| `2da9c53d` | `operator_norm_equivalence` | Operator norm equivalence |

## UUID Index — Paper 2

30 certificate entries across 8 files.

| UUID | Key Theorems | Description |
|------|-------------|-------------|
| `0f05e8c5` | `elsner_spectral_perturbation`, `cycle_operator_lipschitz`, `polynomial_lower_bound` | Core spectral theory infrastructure |
| `1b35d61b` | `exponential_forgetting_decay`, `jordan_chevalley_iterate`, `exponential_beats_polynomial` | Main theorem — exponential forgetting with optimal stepsizes |
| `e566a2cf` | `cycle_identity_on_null`, `active_subspace_spectral_radius`, `forgetting_via_active_subspace` | Active subspace decomposition for overparameterised models |
| `ec56831f` | `submultiplicative_norm`, `lyapunov_exponent_subadditive` | Lyapunov exponent and submultiplicative bounds |
| `87d91033` | `deterministic_beats_stochastic`, `cyclic_lyapunov_negative` | Deterministic cyclic ordering strictly optimal |
| `834259ba` | `commutative_lyapunov_negative` | Commutative Lyapunov exponent negativity |
| `4ee38e9e` | `lyapunov_exponent_lipschitz` | Lyapunov exponent Lipschitz continuity |
| `0141d423` | `markov_cannot_beat_cyclic`, `optimal_ordering_certificate` | Markov chains cannot beat deterministic cyclic ordering |

## UUID Index — Shared

| UUID | Key Theorems | Description |
|------|-------------|-------------|
| `e9d96090` | `curriculum_theorem`, `trace_ordering_optimal` | Curriculum Theorem — cited by both papers |

## Toolchain

- **Prover:** [Aristotle](https://aristotle.harmonic.fun) by [Harmonic](https://harmonic.fun)
- **Language:** Lean 4
- **Library:** [Mathlib](https://github.com/leanprover-community/mathlib4), commit `f897ebcf`

## Citation

If you use these proofs in your work, please cite the papers and this repository:

```bibtex
@misc{hanly2026cyclic,
  author = {Hanly, David G.},
  title = {Closed-Form Optimal Stepsizes for Cyclic Continual Learning:
           The Complete $d=2$ Theory and the Algebraic Boundary at $K=3$},
  year = {2026},
  note = {Preprint}
}

@misc{hanly2026exponential,
  author = {Hanly, David G.},
  title = {Exponential Forgetting Decay via Spectral Stepsize Optimisation
           in Cyclic Continual Learning},
  year = {2026},
  note = {Preprint}
}

@misc{hanly2026proofs,
  author = {Hanly, David G.},
  title = {Formally Verified Proofs for Cyclic Continual Learning},
  year = {2026},
  publisher = {GitHub},
  url = {https://github.com/WellWizard/continual-learning-proofs}
}
```

## License

CC-BY 4.0
