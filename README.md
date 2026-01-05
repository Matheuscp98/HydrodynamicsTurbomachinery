# 🌀 Heat transfer in turbomachinery using Computational Fluid Dynamics

**DOI:** [10.5281/zenodo.18155760](https://doi.org/10.5281/zenodo.18155760)

---

## 📝 Description
The dataset represents a parametric **Computational Fluid Dynamics** (CFD) study of an axial hydraulic turbine inlet duct, modeled in accordance with IEC 60193 recommendations.

Each record corresponds to a CFD simulation conducted according to a **Central Composite Design** (CCD) with **five independent variables** (control factors) and **fourteen dependent variables** (performance metrics).

The dataset is intended for **Statistical Analysis, Response Surface Modeling, Sensitivity Studies, Multiobjetive Optimization (MO), and Machine Learning (ML) applications**.  

**Note:** The main focus of this repository is on the **dataset**.

---

## 📚 Publications

This repository is part of the research study:

-  *Manuscript currently under peer review*

---

## 🛠️ How to Use
1. Clone or download this repository.  
2. Open '.csv' files with **Python (pandas)**, **R**, **Microsoft Excel**, **Google Sheets**, or other software .
5. Use [**Database Heat Transfer**](database.csv) as the **main dataset**.
---

## 📂 Repository Structure

| File | Description |
|------|-------------|
| [**README**](README.md) | Documentation of the dataset and repository usage. |
| [**Database Heat Transfer**](database.csv) | Main dataset. |

---

## 📊 Variables
**Inputs:**
| Symbol | Description | Unit | Range / Levels |
|--------|-------------|------|----------------|
| MV | Mesh volume size | mm | 1.5 – 4.0 |
| ME | Inlet mesh size | mm | 1.5 – 4.0 |
| MS | Outlet mesh size | mm | 1.5 – 4.0 |
| ṁ | Mass flow rate | kg/s | 22.455 – 34.930 |
| CC | Convergence criterion (RMS) | – | 1×10⁻⁵ – 1×10⁻⁴ |


**Outputs:**
| Symbol | Description | Unit |
|--------|-------------|------|
| CM | Mesh generation cost | ×10⁻¹ USD |
| CS | Simulation cost | ×10⁻¹ USD |
| Nel | Number of mesh elements | ×10⁶ |
| Q | Average mesh quality | ×10⁻³ |
| AR | Aspect ratio | ×10⁻⁴ |
| Ortho | Average orthogonality | ×10⁻⁴ |
| Skew | Average skewness | ×10⁻⁴ |
| It | Number of iterations | – |
| VM_RMS | Root Mean Square of vertical momentum | ×10⁶ |
| ΔP | Pressure difference | ×10³ Pa |
| k | Turbulent kinetic energy | ×10¹ m²/s² |
| ε | Turbulence dissipation rate | ×10⁻³ |
| Re | Reynolds number | ×10⁻⁶ |
| y+ | Wall coordinate (dimensionless) | ×10⁻¹ |


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
