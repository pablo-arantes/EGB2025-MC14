# EGB2025-MC14

# 5-Day Course Program: Molecular Docking in the Cloud

This repository contains the materials and schedule for the 5-day course on cloud-based molecular docking.

---

## Day 1 – Introduction to Molecular Docking

### Theory
- **What is molecular docking?**
  - Concepts of binding, scoring functions, and search algorithms.
  - Applications in drug discovery.
- **Limitations and challenges:**
  - Protein flexibility, scoring accuracy, false positives, and sampling issues.

### Hands-on (Google Colab)
- Introduction to Google Colab and Jupyter Notebooks.
- File formats overview: SDF, MOL2, PDBQT.
- Basic input preparation: download one ligand and one protein structure.

1) **Slides:** [Slides](https://github.com/pablo-arantes/EGB2025-MC14/raw/main/EGB%20MC14%20-%20Aula%201.pdf)  - `Introduction to Molecular Docking`
2) **Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pablo-arantes/EGB2025-MC14/blob/main/Regular_Docking_EGB.ipynb)  - `Regular Docking with Vina Scoring Function`
---

## Day 2 – Docking with GNINA: AI-Powered Docking

### Theory
- **Introduction to GNINA:**
  - How convolutional neural networks enhance docking accuracy.
  - Overview of scoring functions: traditional Vina vs. CNN-based scoring.

### Hands-on (Google Colab)
- Install and run GNINA on Colab.
- Dock ligands into the protein target.
- Explore different scoring functions (vina, cnnpose, cnnaffinity, etc.).
- Visualize docking poses with Py3Dmol or NGLView.

1) **Slides** [Slides](https://github.com/pablo-arantes/EGB2025-MC14/raw/main/EGB_MC14_Aula_2_GNINA.pdf)  - `Docking with GNINA: AI-Powered Docking`
2) **Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pablo-arantes/EGB2025-MC14/blob/main/GNINA_EGB_Aula2.ipynb)  - `Docking with GNINA`
---

## Day 3 – Uni-Dock: High-Performance Docking with GPU Acceleration

### Theory
- **Introduction to Uni-Dock:**
  - GPU-accelerated docking for high-throughput screening.
  - When to use Uni-Dock vs. GNINA (speed vs. scoring detail).

### Hands-on (Google Colab with GPU)
- Set up and run Uni-Dock.
- Perform docking of multiple ligands.
- Compare speed and performance between Uni-Dock and GNINA.

1) **Slides** [Slides](https://github.com/pablo-arantes/EGB2025-MC14/raw/main/EGB_MC14_Aula3.pdf)  - `Uni-Dock: High-Performance Docking with GPU Acceleration`
2) **Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pablo-arantes/EGB2025-MC14/blob/main/Uni_Dock_EGB.ipynb)  - `Docking with Uni-Dock`

---

## Day 4 – Virtual Screening: Filters, ADME, and Druglikeness

### Theory
- **Compound selection criteria:**
  - Physicochemical properties relevant to drug design.
  - Lipinski’s Rule of Five, Veber, Ghose, and beyond.
- **Introduction to ADME filters:**
  - Absorption, Distribution, Metabolism, Excretion properties.
- **Importance of filtering to improve virtual screening success.**

### Hands-on (Google Colab)
- **Property calculation:**
  - MW, LogP, H-bond donors/acceptors, TPSA, rotatable bonds.
- Apply physicochemical and ADME filters to a ligand set.
- Prepare a docking-ready ligand library.
- Docking using Uni-Dock or GNINA with the curated set.

1) **Slides** [Slides](https://github.com/pablo-arantes/EGB2025-MC14/blob/main/EGB_MC14_Aula_4_Virtual_Screening.pdf)  - `Virtual Screening: working with compound libraries`
2) **Notebook** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/pablo-arantes/EGB2025-MC14/blob/main/EGB_Virtual_Screening_Aula4.ipynb)  - `Virtual Screening with Gnina`

---

## Day 5 – Post-Docking Analysis and Pose Stability with PLACER

### Theory
- **Post-docking analysis:**
  - How to interpret docking scores.
  - Clustering poses, rescoring, and filtering false positives.
- **Introduction to PLACER:**
  - AI-based tool to predict pose stability.
- **Best practices:**
  - Computational reproducibility in cloud-based environments.

### Hands-on (Google Colab)
- Run PLACER to assess pose stability from GNINA/Uni-Dock outputs.
- Identify and interpret stable vs. unstable docking poses.
- Discuss downstream workflows: MD simulations, free energy calculations, etc.

---

## Summary of Course Flow
- **Day 1:** Understand molecular docking + basic setup.
- **Day 2:** Run AI-powered docking with GNINA.
- **Day 3:** Scale up with GPU-accelerated Uni-Dock.
- **Day 4:** Apply drug-likeness filters, create a ligand library, and finalize the virtual screening pipeline.
- **Day 5:** Validate poses with PLACER (pose stability).

## Acknowledgments
- We would like to thank the [GNINA](https://github.com/gnina/gnina) team for doing an excellent job open sourcing the software.
- We would like to thank the [Uni-Dock](https://github.com/dptech-corp/Uni-Dock) team for doing an excellent job open sourcing the software.
- We would like to thank the [OpenBPMD](https://github.com/Gervasiolab/OpenBPMD) team for their open source implementation of binding pose metadynamics (BPMD).
- We would like to thank the [Roitberg](https://roitberg.chem.ufl.edu/) team for developing the fantastic [TorchANI](https://github.com/aiqm/torchani).
- We would like to thank [@ruiz_moreno_aj](https://twitter.com/ruiz_moreno_aj) for his work on [Jupyter Dock](https://github.com/AngelRuizMoreno/Jupyter_Dock) 
- We would like to thank the ChemosimLab ([@ChemosimLab](https://twitter.com/ChemosimLab)) team for their incredible [ProLIF](https://prolif.readthedocs.io/en/latest/index.html#) (Protein-Ligand Interaction Fingerprints) tool.
- Also, credit to [David Koes](https://github.com/dkoes) for his awesome [py3Dmol](https://3dmol.csb.pitt.edu/) plugin.
- Finally, we would like to thank [Making it rain](https://github.com/pablo-arantes/making-it-rain) team, **Pablo R. Arantes** ([@pablitoarantes](https://twitter.com/pablitoarantes)), **Marcelo D. Polêto** ([@mdpoleto](https://twitter.com/mdpoleto)), **Conrado Pedebos** ([@ConradoPedebos](https://twitter.com/ConradoPedebos)) and **Rodrigo Ligabue-Braun** ([@ligabue_braun](https://twitter.com/ligabue_braun)), for their amazing work.
- A Cloud-Bind by **Pablo R. Arantes** ([@pablitoarantes](https://twitter.com/pablitoarantes))

## How should I reference this work?
- If you’re using **GNINA**, please also cite: <br />
  McNutt et al. "GNINA 1.0: molecular docking with deep learning." <br />
  Journal of Cheminformatics (2021) doi: [10.1186/s13321-021-00522-2](https://doi.org/10.1186/s13321-021-00522-2)
- If you’re using **Uni-Dock**, please also cite: <br />
  Yu et al. "Uni-Dock: GPU-Accelerated Docking Enables Ultralarge Virtual Screening." <br />
  Journal of Chemical Theory and Computation (2023) doi: [10.1021/acs.jctc.2c01145](https://doi.org/10.1021/acs.jctc.2c01145)
- If you’re using **Molecular Dynamics Notebook**, please also cite: <br />
  Arantes et al. "Making it rain: cloud-based molecular simulations for everyone." <br />
  Journal of Chemical Information and Modeling (2021) doi: [10.1021/acs.jcim.1c00998](https://doi.org/10.1021/acs.jcim.1c00998)
