# 🌀 Hydrodynamic System Database

**DOI:** [10.5281/zenodo.18550890](https://doi.org/10.5281/zenodo.18550890)

---

## 📝 Description
This repository provides a structured experimental–numerical dataset for a  **hydrodynamic system composed of an axial hydraulic turbine inlet duct with bulb**, developed in accordance with IEC 60193 recommendations.

The dataset combines **experimentally measured reference data** obtained from a reduced-scale hydraulic test bench with **numerical results generated through Computational Fluid Dynamics (CFD)** simulations organized via a **Central Composite Design (CCD)**.

Each numerical record corresponds to a CFD simulation defined by **five independent control variables** (mesh configuration, mass flow rate, and convergence criterion) and a comprehensive set of **numerical response variables** describing mesh quality, convergence behavior, computational cost, and hydrodynamic performance.

Experimental measurements are used as **physical target values** to support validation, error analysis, and numerical strategy assessment.

The dataset is intended for:
- Statistical Analysis;
- Design of Experiments (DOE);
- Response Surface Methodology (RSM);
- Sensitivity Analysis;
- Multi-objective Optimization (MO);
- Machine Learning (ML) applications.

**Note:** The primary focus of this repository is the dataset itself. No proprietary CFD setup or software is required to reuse the data.

---

## 📚 Publications

This repository is associated with the following research work:

-  *Manuscript currently under peer review*

---

## 🛠️ How to Use

1. Clone or download this repository.  
2. Open the `.csv` files using **Python (pandas)**, **MATLAB**, **R**, **Microsoft Excel**, **Google Sheets**, or equivalent tools.  
3. Use the datasets as follows:

- [**CFD Data**](CFD_data.csv): Numerical data for modeling and optimization  
- [**Experimental Data**](experimental_data.csv): Experimental measurements used as physical reference targets  
- [**Metadata Variables**](metadata_variables.csv): Complete metadata for all variables (units, meaning and classification)

---

## 📂 Repository Structure

| File | Description |
|------|-----------|
| [**README**](README.md) | Documentation of the dataset, structure, and usage guidelines. |
| [**CFD Data**](CFD_data.csv) | Numerical results obtained from CFD simulations organized according to a Central Composite Design. |
| [**Experimental Data**](experimental_data.csv) | Experimentally measured reference values used as physical targets for validation. |
| [**Metadata Variables**](metadata_variables.csv) | Complete metadata describing all variables, including abbreviations, units, physical meaning, and classification (input, output, target). |

---

## 📊 Variables

### 🔹 Input Variables

| Symbol | Description | Unit | Range / Levels |
|-------|------------|------|----------------|
| MV | Global mesh volume size | mm | 1.5 – 4.0 |
| ME | Inlet mesh size | mm | 1.5 – 4.0 |
| MS | Outlet mesh size | mm | 1.5 – 4.0 |
| ṁ | Mass flow rate | kg/s | 22.455 – 34.930 |
| CC | Convergence criterion (RMS residual threshold) | – | 1×10⁻⁵ – 1×10⁻⁴ |

---

### 🔹 Output Variables (CFD)

| Symbol | Description | Unit |
|-------|------------|------|
| CM | Mesh generation cost | ×10⁻¹ USD |
| CS | CFD simulation cost | ×10⁻¹ USD |
| Nel | Number of mesh elements | ×10⁶ |
| Q | Mean mesh quality indicator | ×10⁻³ |
| AR | Mean aspect ratio | ×10⁻⁴ |
| Ortho | Mean mesh orthogonality | ×10⁻⁴ |
| Skew | Mean mesh skewness | ×10⁻⁴ |
| It | Number of solver iterations | – |
| VM_RMS | RMS of velocity residuals | ×10⁶ m/s |
| ΔP | Numerical pressure drop | ×10³ Pa |
| k | Turbulent kinetic energy | m²/s² |
| ε | Turbulent dissipation rate | m²/s³ |
| Re | Numerical Reynolds number | ×10⁶ |
| y⁺ | Wall coordinate | – |

---

### 🔹 Experimental Variables (Measured)

| Symbol | Description | Unit |
|-------|------------|------|
| v | Mean flow velocity | m/s |
| P_inlet | Inlet pressure | ×10³ Pa |
| P_outlet | Outlet pressure | ×10³ Pa |

---

### 🎯 Target Variables (Experimental References)

| Symbol | Description | Unit |
|-------|------------|------|
| ΔP_target | Adjusted experimental pressure drop (bulb domain) | ×10³ Pa |
| Re_target | Experimental Reynolds number | ×10⁶ |

---

## 📄 Metadata

All variables are fully documented in **metadata_variables.csv**, including:

- Abbreviations  
- Units (SI)  
- Physical meaning  
- Classification (input, output, target)  
- Data source (CFD or experimental)

This metadata enables direct reuse of the dataset without access to the original CFD setup or laboratory infrastructure.

---

## 📌 Notes on Data Organization

- Numerical and experimental data are provided in separate files to clearly distinguish measured values from simulation-derived results.  
- All variables, scaling factors, and units are fully described in **metadata_variables.csv**, ensuring correct interpretation without requiring access to proprietary CFD software or the original simulation setup.  
- Reported numerical values correspond to statistically processed outputs (mean values), supporting reproducibility and response-level comparison.
---

## License
This dataset is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0).  
See the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

<a href="mailto:matheusc_pereira@hotmail.com">
  <img src="https://i.ibb.co/k6Ddn36k/email.png" alt="E-mail" height="60"/>
</a>
<a href="https://www.linkedin.com/in/matheuscostapereira/">
  <img src="https://i.ibb.co/Kx4rZxdr/linkedin.png" alt="LinkedIn" height="60"/>
</a>
<a href="https://scholar.google.com.br/citations?user=1iDBIzYAAAAJ&hl=en-us">
  <img src="https://i.ibb.co/SwsRKK1t/scholar.png" alt="Google Scholar" height="60"/>
</a>
<a href="https://lattes.cnpq.br/7025666927284220">
  <img src="https://i.ibb.co/1fMjS38j/lattes.png" alt="Lattes" height="60"/>
</a>

---

> _Feel free to open issues or PRs, or reach out for collaboration or questions!_
