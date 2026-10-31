
# Additional Benchmark Instances for Operating Room Scheduling

## 1. Project Overview

This repository provides a Python script for generating additional benchmark instances (Instances 11–20) for the **Operating Room Scheduling Problem (ORSP)**.

The generated instances are based on the structure of the original benchmark dataset presented in the following research article:

**Reference article:**

* A Bi-Objective Stochastic Model for Operating Room Scheduling Considering Surgeons’ Preferences and Collaborative Surgeries.*

**Authors:** Rana Azab, Amr Eltawil, and Mohamed Gheith (2025).

The main objective of generating these additional instances is to extend the available benchmark dataset and provide further test instances for evaluating optimization algorithms, particularly the **Cuckoo–Catfish Optimizer (CCO)**.

**Important:** Instances 11–20 are additional instances generated for this research project. They are not part of the original dataset published in the reference article.

## 2. Repository Contents

The repository is organized as follows:

```text
CCO-OR-Scheduling/
│
├── instances/
│   ├── Instance 1.xlsx
│   ├── Instance 2.xlsx
│   ├── ...
│   ├── Instance 10.xlsx
│   ├── Instance 11.xlsx
│   ├── ...
│   └── Instance 20.xlsx
│
├── generate_instances_11_20.py
│
└── README.md
```

- **Original instances (1–10):** Benchmark instances from the reference dataset, subject to its redistribution conditions.
- **Generated instances (11–20):** Additional benchmark instances generated using the provided Python script.
- **`generate_instances_11_20.py`:** Python script responsible for generating the additional instances.

## 3. Requirements

The instance-generation script requires:

- Python 3.x
- `openpyxl`

Install the required library using:

```bash
pip install openpyxl
```

## 4. Generating the Additional Instances

To generate Instances 11–20, follow these steps:

**Step 1.** Clone or download this repository.

**Step 2.** Make sure the original template file, `Instance 1.xlsx`, is available in the same directory as the generation script, unless the script is configured to use another path.

**Step 3.** Install the required Python dependency:

```bash
pip install openpyxl
```

**Step 4.** Execute the generator:

```bash
python generate_instances_11_20.py
```

The script generates the additional Excel benchmark files (Instances 11–20).

## 5. Reproducibility

The instance-generation procedure uses predefined random seeds to support reproducibility.

Using the same template, generation script, configuration, and random seeds allows the generated instances to be reproduced.

For reproducibility of the optimization experiments, the random seeds used for the independent algorithm runs should also be recorded separately.

The experimental protocol considers 30 independent runs per instance. The seeds and corresponding experimental results should be made available alongside the experiment code when published.

## 6. Experimental Evaluation

The additional instances are intended to evaluate the performance of the Cuckoo–Catfish Optimizer (CCO) on the Operating Room Scheduling Problem.

The experimental evaluation considers the following performance indicators:

- Best objective value.
- Mean objective value.
- Standard deviation.
- Computational runtime.
- Feasibility of the obtained solutions.

The additional instances provide further test scenarios for examining the performance and robustness of the optimization approach.

## 7. Citation

If you use the original benchmark formulation or dataset, please cite the following article:

Azab, R., Eltawil, A., & Gheith, M. (2025). A bi-objective stochastic model for operating room scheduling considering surgeons’ preferences and collaborative surgeries. *Decision Analytics Journal, 14*, 100544.

**DOI:** https://doi.org/10.1016/j.dajour.2024.100544

**BibTeX:**

```bibtex
@article{17,
  author = {Azab, Rana and Eltawil, Amr and Gheith, Mohamed},
  year = {2025},
  month = {03},
  pages = {100544},
  title = {A bi-objective stochastic model for operating room scheduling considering surgeons’ preferences and collaborative surgeries},
  volume = {14},
  journal = {Decision Analytics Journal},
  doi = {10.1016/j.dajour.2024.100544}
}
```

## 8. Dataset Attribution and Usage

The original benchmark instances and the additional generated instances are distinct datasets and should be identified accordingly.

The additional instances (11–20) were generated specifically for this research project using the provided Python script.

Users of this repository should cite the original research article when using its benchmark formulation or original dataset and clearly acknowledge the generated instances when using Instances 11–20.

Please respect the original dataset's licensing and redistribution conditions.
