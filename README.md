# Awesome Magnetic Materials & AI

> A curated collection of software, datasets, machine-learning models, simulators, and visualization tools for magnetic materials research.

**Scope:** computational magnetism, magnetic-property prediction, experimental magnetometry, spin simulations, crystal generation, magnetic data, and relevant adjacent tools.  
**Important:** a tool that supports crystal structures or magnetic *fields* does not automatically predict intrinsic magnetic order, Curie temperature, or exchange bias.

## Contents

- [Magnetic-property prediction and ML](#magnetic-property-prediction-and-ml)
- [First-principles magnetism, Hamiltonians and workflows](#first-principles-magnetism-hamiltonians-and-workflows)
- [Atomistic spin and micromagnetics](#atomistic-spin-and-micromagnetics)
- [Spin waves and magnetic excitations](#spin-waves-and-magnetic-excitations)
- [Experimental magnetometry and analysis](#experimental-magnetometry-and-analysis)
- [Scientific visualization](#scientific-visualization)
- [Databases, data access and benchmarks](#databases-data-access-and-benchmarks)
- [Crystal generation and screening](#crystal-generation-and-screening)
- [Related: applied magnetic fields and engineering](#related-applied-magnetic-fields-and-engineering)

## Using the catalog

- **Input:** composition, crystallographic structure (CIF / mCIF), DFT results, spin Hamiltonian, experimental magnetometry, or field geometry.
- **Output:** Tc/TN, magnetic class, local moments, exchange couplings, simulated magnetization, hysteresis, magnon dispersion, or graphics.
- **Verification:** descriptions are based on publicly documented project purposes; this file does **not** imply the project has been installed, benchmarked, or checked for research reproducibility.
- **Licensing and maintenance:** consult each upstream repository before use; a GitHub URL is not a license to redistribute code.
- **Origin tags:** `new` = added in this curation; `seed` = included in the initial list.

## Magnetic-property prediction and ML

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [CurieML](https://github.com/Songyosk/CurieML) | Composition-based machine learning workflows for Curie-temperature prediction. | Tc · composition · ML | seed |
| [NEMAD-MagneticML](https://github.com/sumanitani/NEMAD-MagneticML) | Models and datasets for Tc, Néel temperature and FM/AFM/NM classification. | Tc · TN · order · ML | new |
| [MagBERT / NLP_magnets](https://github.com/ucarh/NLP_magnets) | NLP workflows for extracting Curie-temperature information from literature. | NLP · data extraction | new |
| [Exchange bias ML](https://github.com/kwillon/Magnet_Exchange_bias) | Research code for predicting exchange bias in magnetic materials; inspect its assumptions and data before reuse. | exchange bias · ML | seed |
| [Iron-based nanocrystalline alloy design](https://github.com/yuhaowang2018/Machine_learning_approach_to_Iron_based_soft_magnetic_nanocrystalline_materials_design) | Research workflow for ML-guided design of Fe-based soft magnetic nanocrystalline alloys. | soft magnets · alloy ML | seed |
| [CHGNet](https://github.com/CederGroupHub/chgnet) | Pretrained interatomic potential predicting energy, forces, stress and site magnetic-moment magnitudes; not a universal magnetic-order oracle. | CIF · site moments · ML | new |
| [ALIGNN](https://github.com/usnistgov/alignn) | Atomistic line-graph neural network; includes a magnetic/non-magnetic classification example and general material regressors. | GNN · classifier | new |
| [CGCNN](https://github.com/txie-93/cgcnn) | Crystal graph network customizable for magnetic property prediction with suitable labelled data. | CIF · GNN · trainable | new |
| [MEGNet](https://github.com/materialyzeai/megnet) | General graph-network architecture for structure–property modeling; magnetic targets require suitable training data. | GNN · trainable | seed |
| [matminer](https://github.com/hackingmaterials/matminer) | Materials science featurizers and data-mining tools for composition/structure/property modeling. | descriptors · ML | new |
| [scikit-mol](https://github.com/EBjerrum/scikit-mol) | Molecular featurization for scikit-learn; relevant to molecular magnets rather than inorganic crystals. | molecular ML | seed |
| [AtomGPT](https://github.com/atomgptlab/atomgpt) | Transformer-based framework for forward property prediction and inverse materials design. | LLM · materials | new |

## First-principles magnetism, Hamiltonians and workflows

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [TB2J](https://github.com/mailhexu/TB2J) | Compute exchange couplings, anisotropic exchange and DMI from DFT-derived Hamiltonians. | DFT → Jij · DMI | seed |
| [TB2J examples](https://github.com/mailhexu/TB2J_examples) | Worked DFT/Wannier/TB2J calculations for FeO, SrMnO3, CrI3 and more. | tutorial · exchange | new |
| [MagneticTB](https://github.com/zhangzeyingvv/MagneticTB) | Symmetry-adapted tight-binding Hamiltonian models for magnetic materials. | magnetic symmetry · TB | seed |
| [pymatgen](https://github.com/materialsproject/pymatgen) | Structure I/O, magnetic ordering analysis and enumeration, Heisenberg mapping, spin-aware utilities. | CIF · magmom · structure | seed |
| [atomate2](https://github.com/materialsproject/atomate2) | Automated atomistic workflows, including magnetic ordering workflows for DFT calculations. | HPC · DFT automation | new |
| [AiiDA](https://github.com/aiidateam/aiida-core) | Workflow and provenance engine for reproducible high-throughput calculations. | automation · provenance | new |
| [Quantum ESPRESSO](https://gitlab.com/QEF/q-e) | Open-source electronic structure DFT code with spin-polarized/noncollinear calculation capabilities. | DFT · spin | new |
| [MAGNDATASymData](https://github.com/FengTang1990/MAGNDATASymData) | Symmetry-related high-symmetry point information for magnetic materials from MAGNDATA. | symmetry | seed |
| [ToMSGKpoint](https://github.com/FengTang1990/ToMSGKpoint) | Magnetic-space-group-related k-point utility; review its supported inputs before use. | k-points · MSG | seed |
| [curie_calculator [unmaintained]](https://github.com/Volkov-da/curie_calculator) | Research prototype for magnetic critical-temperature calculation; its README says VASP is required and the project is unsupported. | Tc · VASP · legacy | seed |

## Atomistic spin and micromagnetics

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [VAMPIRE](https://github.com/richard-evans/vampire) | Atomistic spin model simulations for temperature-dependent magnetization, hysteresis and magnetic dynamics. | atomistic · dynamics | seed |
| [Spirit](https://github.com/spirit-code/spirit) | Atomistic Heisenberg spin simulation, LLG, DMI, energy barriers and interactive 3D spin visualization. | atomistic · GUI | new |
| [UppASD](https://github.com/UppASD/UppASD) | Atomistic spin dynamics and Monte Carlo; critical temperatures and magnon spectra. | atomistic · Tc · magnons | new |
| [Fidimag](https://github.com/computationalmodelling/fidimag) | Python-facing finite-difference micromagnetic and atomistic simulations, including LLG and transition paths. | micro · atomistic | new |
| [MuMax3](https://github.com/mumax/3) | GPU finite-difference micromagnetics for domain configurations, switching and dynamics. | micromagnetics · CUDA | new |
| [mumax+](https://github.com/mumax/plus) | Extensible GPU-accelerated micromagnetics with a Python interface. | micromagnetics · GPU | new |
| [Ubermag](https://github.com/ubermag/ubermag) | Python/Jupyter front end for micromagnetics using external solvers such as OOMMF and MuMax3. | Jupyter · workflow | new |
| [Boris2](https://github.com/SerbanL/Boris2) | Multiphysics micromagnetic/spintronics simulation environment. | spintronics · micro | seed |
| [MagTense](https://github.com/cmt-dtu-energy/MagTense) | Micromagnetic and magnetostatic models using analytical demagnetization tensors. | micro · field | new |
| [SpinTorch](https://github.com/a-papp/SpinTorch) | PyTorch-based micromagnetics for optimization and machine learning with spin waves. | differentiable · spin waves | new |
| [NeuralMag](https://gitlab.com/neuralmag/neuralmag) | Differentiable GPU micromagnetics with JAX/PyTorch; particularly useful for inverse problems. | differentiable · micro | new |

## Spin waves and magnetic excitations

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [Sunny.jl](https://github.com/SunnySuite/Sunny.jl) | Symmetry-aware spin Hamiltonians, spin waves, quantum effects and scattering simulation in Julia. | magnons · quantum | new |
| [SpinW](https://github.com/spinw/SpinW) | MATLAB code for magnetic structure optimization, spin-wave dispersions and scattering. | magnons · MATLAB | new |
| [pySpinW](https://github.com/SpinW/pySpinW) | Python implementation of SpinW; check development status and available features. | magnons · Python | new |

## Experimental magnetometry and analysis

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [HYLOA](https://github.com/Francesco-Zeno-Costanzo/hyloa) | Desktop app to import, correct, analyze and visualize magnetic hysteresis loops. | M-H · experiments | new |
| [Magnetometry Analysis App](https://github.com/BRimmler/Magnetometry-Analysis-App) | Analysis scripts for SQUID-VSM/Lake Shore M(H) and M(T), background subtraction and magnetic moment normalization. | M-H · M-T · SQUID | new |
| [PBenderLux Data-analysis](https://github.com/PBenderLux/Data-analysis) | Research-specific data-analysis code; inspect the associated experiments before adopting methods. | experimental scripts | seed |

## Scientific visualization

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [Crystal Toolkit](https://github.com/materialsproject/crystaltoolkit) | Web components for crystal structures including visualizing site magnetic moments. | CIF · spins · web | new |
| [MatterViz](https://github.com/janosh/matterviz) | Interactive 3D crystal/trajectory and structure-property visualizations, including a VS Code viewer. | 3D · CIF · browser | new |
| [pymatviz](https://github.com/janosh/pymatviz) | Plotting utilities for materials informatics, data/property distributions and crystal views. | plots · materials | new |
| [PyVista](https://github.com/pyvista/pyvista) | General-purpose 3D mesh and vector field rendering for magnetization arrows, textures and simulation grids. | 3D · vectors · VTK | new |
| [discretisedfield](https://github.com/ubermag/discretisedfield) | Numerical scalar/vector-field handling, OVF/VTK files and magnetization plotting. | OVF · vector field | new |
| [spinView](https://github.com/spirit-code/spinView) | Desktop post-processing viewer for spin-simulation results. | spins · GUI | new |
| [vaspMagtools](https://github.com/kantaimperial/vaspMagtools) | Convert VASP OUTCAR local moments to mCIF for VESTA, or reuse moments as MAGMOM input. | DFT · mCIF · arrows | new |
| [Magpylib](https://github.com/magpylib/magpylib) | Model and visualize the fields of magnets, currents and dipoles; primarily magnetostatics. | H/B field | seed |
| [Fields](https://github.com/mlhoutel/Fields) | Electromagnetic field visualization; relevant to field maps rather than intrinsic magnetic ordering. | electromagnetism · visuals | seed |
| [OVITO](https://www.ovito.org/) | Particle/atomistic trajectory visualization with scripting; desktop tiers have different licensing. | particles · trajectories | new |

## Databases, data access and benchmarks

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [MAGNDATA](https://www.cryst.ehu.eus/magndata/) | Published experimental magnetic structures (mCIF), including magnetic symmetry and spin configurations. | magnetic structures · mCIF | new |
| [Materials Project API](https://github.com/materialsproject/api) | Retrieve crystal structures and available computed properties / magnetism metadata from Materials Project. | API · structures | new |
| [JARVIS-Tools](https://github.com/usnistgov/jarvis) | Access and process diverse NIST-JARVIS materials and computation datasets. | dataset · DFT | new |
| [GNoME / materials_discovery](https://github.com/google-deepmind/materials_discovery) | Data and models for inorganic crystal discovery; not a magnetism-specific predictor. | candidate structures | seed |
| [Princeton MagNet](https://github.com/PrincetonUniversity/magnet) | Magnetic-core losses and power-electronics magnetics data; distinct from atomistic spin-order prediction. | power magnetics | seed |
| [MagNet Challenge](https://github.com/minjiechen/magnetchallenge-1) | Challenge data/models for power magnetics and core losses, not atomic-scale magnetism. | power magnetics | seed |

## Crystal generation and screening

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [MatterGen](https://github.com/microsoft/mattergen) | Generative inorganic crystal model with property-conditioned fine-tuning. | generative · CIF | new |
| [SMACT](https://github.com/WMD-group/SMACT) | Composition screening using chemistry-informed plausibility and charge-balance checks. | composition screening | new |
| [Crystal-generator-using-SLICES](https://github.com/shtnpd/Crystal-generator-using-SLICES) | Crystal generation based on the SLICES structural representation; general-purpose research prototype. | generative · structures | seed |
| [nanoMINER](https://github.com/ai-chem/nanoMINER) | Multimodal/LLM extraction of nanomaterials information from research papers. | literature · extraction | seed |
| [Nanomaterial Morphology Prediction](https://github.com/ai-chem/Nanomaterial_Morphology_Prediction) | Research workflows for nanomaterial morphology prediction rather than magnetism itself. | nanomaterial · morphology | seed |

## Related: applied magnetic fields and engineering

| Project | What it does | Keywords | Origin |
|---|---|---|---|
| [bmapping-pinn](https://github.com/ucoskun/bmapping-pinn) | Physics-informed neural network for reconstructing spatial magnetic fields from measurements. | PINN · field mapping | seed |
| [FEMM](https://github.com/cenit/FEMM) | Finite-element electromagnetics and magnetostatics for device and geometry design. | FEM · magnets | seed |
| [pycurious](https://github.com/brmather/pycurious) | Geophysical estimation of magnetic Curie-point depth from magnetic anomalies, not material Tc. | geophysics | seed |

## Important exclusions and scope notes

Keep unrelated software outside the central magnetic-materials index (or in a separate `adjacent/` list): speech recognition (Vosk), AI interview assistants, generic language-model tutorials, ocean-temperature tutorials, MRI reconstruction tools, plasma equilibrium tools, generic energy-system toolkits, electronic badge spoofing, etc.

**Terminology matters:** (a) Curie *depth* from geophysical anomalies ≠ material Curie *temperature*; (b) magnetic-core loss modeling ≠ atomistic spin-order prediction; (c) field-mapping ≠ predicting intrinsic magnetic properties.

## Suggested contribution template

To propose an addition, provide:

```text
Project name:
URL:
Category:
Inputs:
Outputs:
Material scale: electronic / atomistic / continuum / device
License:
Last checked (YYYY-MM-DD):
Evidence (paper/docs):
Limitations:
```

## How to cite

Please cite original software publications and datasets, not this index alone.

_Initial curated draft: 2026-10-22._
