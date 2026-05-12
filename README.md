# ob_gain_control_decorrelation

Welcome to the ob_gain_control_decorrelation repo.

This repository contains analysis code and datasets supporting our study:

**Decorrelation by gain control in the mouse olfactory bulb**  

<a href="https://www.biorxiv.org/cgi/content/short/2026.05.07.722633v1" target="_blank" rel="noopener noreferrer">
Preprint link
</a>
---

## 🔎 The story

How does the olfactory bulb transform sensory input from olfactory sensory neurons into representations that are easier to discriminate?

In this study, we quantified how odour representations are decorrelated from sensory input to olfactory bulb output and identified the circuit motifs capable of implementing this transformation.

To do this, we combined:

- **Two-photon calcium imaging** of OSN input (OMP-GCaMP6f) and mitral/tufted cell output (Tbet-GCaMP6f) across matched dorsal OB fields,  
- **A computational model** of the olfactory bulb input–output transformation to test candidate connectivity motifs,  
- **Comparative analysis** of correlation structure, representational dimensionality, and decoding performance across representations.

### Key findings

- 📉 **Output representations are decorrelated** relative to sensory inputs, increasing odour separability.  
- 📈 Output activity occupies a **higher-dimensional representation space** and supports improved odour decoding accuracy.  
- 🧩 Most of the observed decorrelation can be explained by **channel-specific gain modulation**, without requiring extensive lateral inhibition.  
- 🧠 Recordings from M/T cell somata confirmed that decorrelation is preserved across layers and behavioural states.  
- 🧮 Linear modelling revealed that low-dimensional connectivity motifs and feedforward scaling capture the majority of the experimentally observed transformations.  

Together, these results suggest that feedforward gain control is a major mechanism by which the olfactory bulb reshapes sensory representations to improve odour discriminability.

---

## 👩‍💻 Getting started

Clone this repository:

```bash
git clone https://github.com/ackels-lab/ob_gain_control_decorrelation.git
cd ob_gain_control_decorrelation
```

Set up the environment using the provided `environment.yml` file:

```bash
conda env create -f environment.yml
conda activate ob_io_env
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open and run the main notebook:

```bash
notebooks/IO_main_figures.ipynb
```

This notebook reproduces the key panels of the main figures.  
(Additional scripts and figure panels will be released after peer review.)

---

## 📦 Data access

Raw data (`.h5`) files are automatically downloaded via the notebook and are hosted on Zenodo:

👉 https://doi.org/10.5281/zenodo.17359151

Available datasets include:

- `glom_omp_data.h5`  
  https://zenodo.org/record/17359151/files/glom_omp_data.h5

- `glom_tbet_data.h5`  
  https://zenodo.org/record/17359151/files/glom_tbet_data.h5

- `processed_data.h5`  
  https://zenodo.org/record/17359151/files/processed_data.h5

---

## 🔗 Related repositories

Accompanying repositories covering the computational and modelling components of the study can be found here:

- Repository for connectivity modelling and representational analysis:  
  https://github.com/stootoon/ob_io_conn_models

- Repository for glomerular input–output transformation analysis and modelling tools:  
  https://github.com/stootoon/glom-io-transform-release

These repositories contain additional code for:

- Linear modelling of olfactory bulb input–output transformations  
- Connectivity-constrained decorrelation models  
- Representational geometry analyses  
- Simulation and fitting procedures used throughout the study

---

## 🙌 Acknowledgements

This work was supported by the Francis Crick Institute, University College London, and the University of Bonn, and benefited from discussions with colleagues in physiology, systems neuroscience, and computational modelling.

Please refer to the manuscript for full author contributions and funding details.

---

## ☎️ Contact

For questions, data access, or collaboration inquiries, contact:

**Tobias Ackels**  
tobias.ackels@ukbonn.de

**Andreas T. Schaefer**  
andreas.schaefer@crick.ac.uk

**Sina Tootoonian**  
sina.tootoonian@crick.ac.uk
