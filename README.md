# Data for “Current Induced Switching of Superconducting Order and Enhancement of Superconducting Diode Efficiency”

This repository contains the numerical data associated with the manuscript

**“Current Induced Switching of Superconducting Order and Enhancement of Superconducting Diode Efficiency”**

by **Uddalok Nag, Jonathan Schirmer, Chao-Xing Liu, and J. K. Jain**.

The manuscript has been accepted for publication in *Physical Review B*.

This repository contains **data only**. Numerical, analysis, and plotting codes are not included.

## Data format

All numerical data are stored as MATLAB `.mat` files.

The files contain the following variables:

- `q` — momentum parameter $q$
- `Jq` — supercurrent as a function of $q$
- `Econ` — condensation energy as a function of $q$
- `Psi_1` — superconducting order-parameter amplitude in layer 1
- `Psi_2` — superconducting order-parameter amplitude in layer 2
- `rho` — interlayer-vortex density

Each filename records the parameters used in that calculation. For example,

```text
alpha=-10 beta=20 J=2 m=1 qb=1.85.mat
```

contains data for $\alpha=-10$, $\beta=20$, $J=2$, $m=1$, and $q_B=1.85$.

For asymmetric bilayers, the folders labeled `dalph` use

$$
\alpha_1=\alpha+\delta\alpha,\qquad
\alpha_2=\alpha-\delta\alpha,
$$

where `dalph` denotes $\delta\alpha$. The asymmetry parameter used in the manuscript is

$$
a=\left|\frac{\alpha_1-\alpha_2}{\alpha_1+\alpha_2}\right|.
$$

For $\alpha=-10$, the folders therefore correspond to

- `dalph=0` → $a=0$
- `dalph=1` → $a=0.1$
- `dalph=1.5` → $a=0.15$
- `dalph=2` → $a=0.2$

## Repository structure

```text
Data/
├── Fig1/
├── Fig2/
│   ├── dalph=0/
│   └── dalph=1/
└── Fig3/
    ├── dalph=1/
    ├── dalph=1.5/
    └── dalph=2/
```

### `Data/Fig1/`

Data underlying Fig. 1 of the manuscript.

This directory contains the calculations at

- $q_B=0.6$
- $q_B=1.85$
- $q_B=4.6$

for the parameters used in Fig. 1.

### `Data/Fig2/`

Data underlying the phase diagrams in Fig. 2.

- `dalph=0/` contains data for the symmetric bilayer, $a=0$.
- `dalph=1/` contains data for the asymmetric bilayer, $a=0.1$.

Each directory contains data for the range of \(q_B\) values used to construct the corresponding phase diagram.

### `Data/Fig3/`

Data underlying Fig. 3.

The three directories correspond to the asymmetry values shown in the figure:

- `dalph=1/` → $a=0.1$
- `dalph=1.5/` → $a=0.15$
- `dalph=2/` → $a=0.2$

Each directory contains data for the range of \(q_B\) values used to obtain the superconducting diode efficiency and interlayer-vortex-density results.

## Manuscript parameters

The data in this repository use the Ginzburg–Landau parameters described in the manuscript. The filenames explicitly record the principal parameters for each calculation.

The quantities and conventions used here are defined in the manuscript. In particular, $q_B$ parametrizes the in-plane magnetic field, $E_{\rm con}$ is the condensation energy, and $\rho$ is the interlayer-vortex density.

## Citation

## Citation

If you use these data, please cite the associated article:

> U. Nag, J. Schirmer, C.-X. Liu, and J. K. Jain, “Current Induced Switching of Superconducting Order and Enhancement of Superconducting Diode Efficiency,” *Physical Review B* (2026). https://doi.org/10.1103/xtsd-hkdw

A permanent dataset DOI will be added here after archival.

## Contact

For questions about the data, please contact the authors of the associated manuscript.
